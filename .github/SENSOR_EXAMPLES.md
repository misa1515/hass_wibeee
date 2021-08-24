# Suggested sensor configurations

Some example sensor configurations to get you started with the Wibeee integration
into Home Assistant.

## Power sensors

Wibeee exposes `*_active_power` (a non-negative number) and `*_power_factor` (ranging from -1 to 1) but 
if we want to graph power with positive/negative axis we need to create a new sensor for this.

We also create two separate sensors for integrations that expect non-negative numbers, one for importing from 
the grid and another for exporting to the grid.

In the examples below substitute `phase4` for the desired phase.

```yaml
sensor:
  - platform: template
    sensors:
      #####################
      # Power sensors (W) #
      #####################
      grid_import_export_power:   
        friendly_name: "Grid import(+) or export(-) power"
        device_class: power
        unit_of_measurement: 'W'
        value_template: >-
            {% if states('sensor.wibeee_phase4_power_factor') | float < 0 %}
              {{ states('sensor.wibeee_phase4_active_power') | float * -1 | round(0) }}
            {% else %}
              {{ states('sensor.wibeee_phase4_active_power') | float | round(0) }}
            {% endif %}
      grid_import_power:
        friendly_name: "Grid import power"
        device_class: power
        unit_of_measurement: 'W'
        value_template: "{{ states('sensor.grid_import_export_power') | float | max(0) | round(0) }}"
      grid_export_power:
        friendly_name: "Grid export power
        device_class: power
        unit_of_measurement: 'W'
        value_template: "{{ states('sensor.grid_import_export_power') | float | min(0) | abs | round(0) }}"
```

## Energy sensors

Power sensors give us an instant value of power being imported or exported but not the total amount
of energy in kWh. To calculate the energy we will use the [`integration` platform](https://www.home-assistant.io/integrations/integration/#energy)
to calculate the Riemann Sum of the power series.

```yaml
sensor:
  ########################
  # Energy sensors (kWh) #
  ########################
  - platform: integration
    source: sensor.grid_import_power
    name: grid_import_energy
    unit_prefix: k
    round: 2
  - platform: integration
    source: sensor.grid_export_power
    name: grid_export_energy
    unit_prefix: k
    round: 2
```

The above sensors can be used in the [your Energy Configuration](https://my.home-assistant.io/redirect/config_energy/) to integrate with [Home Energy Management](https://www.home-assistant.io/home-energy-management/).
