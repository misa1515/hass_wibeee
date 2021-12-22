# Changelog

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

## [3.0.0-beta.6](https://github.com/luuuis/hass_wibeee/compare/v3.0.0-beta.5...v3.0.0-beta.6) (2021-12-22)

## [3.0.0-beta.5](https://github.com/luuuis/hass_wibeee/compare/v3.0.0-beta.4...v3.0.0-beta.5) (2021-12-22)

## [3.0.0-beta.4](https://github.com/luuuis/hass_wibeee/compare/v2.2.3...v3.0.0-beta.4) (2021-12-21)


### ⚠ BREAKING CHANGES

* sets `unique_id` on entities, which causes HA to create new entities. Opt out by using `unique_id: false` on the integration.

### Features

* generate entity unique_id from MAC address ([#12](https://github.com/luuuis/hass_wibeee/issues/12)) ([1f8b966](https://github.com/luuuis/hass_wibeee/commit/1f8b966612b3acfb296acde5975fd96d66f3ce9b))
* use human-friendly name for sensors with unique_id, otherwise keep the old name ([#13](https://github.com/luuuis/hass_wibeee/issues/13)) ([bb59ccb](https://github.com/luuuis/hass_wibeee/commit/bb59ccbe518264c336c465ad5fd34521cbac0b12))
* use Wibeee device name to assign Home Assistant name ([#18](https://github.com/luuuis/hass_wibeee/issues/18)) ([da3174c](https://github.com/luuuis/hass_wibeee/commit/da3174c1e9704fe816f533ef359d8469b738e380))


### Bug Fixes

* don't update entities that are disabled ([#15](https://github.com/luuuis/hass_wibeee/issues/15)) ([6474db6](https://github.com/luuuis/hass_wibeee/commit/6474db64ae02642b8e40b5df331d093181401b07))

## [3.0.0-beta.3](https://github.com/luuuis/hass_wibeee/compare/v2.2.3...v3.0.0-beta.3) (2021-12-19)


### ⚠ BREAKING CHANGES

* sets `unique_id` on entities, which causes HA to create new entities. Opt out by using `unique_id: false` on the integration.

### Features

* generate entity unique_id from MAC address ([#12](https://github.com/luuuis/hass_wibeee/issues/12)) ([1f8b966](https://github.com/luuuis/hass_wibeee/commit/1f8b966612b3acfb296acde5975fd96d66f3ce9b))
* use human-friendly name for sensors with unique_id, otherwise keep the old name ([#13](https://github.com/luuuis/hass_wibeee/issues/13)) ([bb59ccb](https://github.com/luuuis/hass_wibeee/commit/bb59ccbe518264c336c465ad5fd34521cbac0b12))
* use Wibeee device name to assign Home Assistant name ([#18](https://github.com/luuuis/hass_wibeee/issues/18)) ([da3174c](https://github.com/luuuis/hass_wibeee/commit/da3174c1e9704fe816f533ef359d8469b738e380))


### Bug Fixes

* don't update entities that are disabled ([#15](https://github.com/luuuis/hass_wibeee/issues/15)) ([6474db6](https://github.com/luuuis/hass_wibeee/commit/6474db64ae02642b8e40b5df331d093181401b07))

## [3.0.0-beta.2](https://github.com/luuuis/hass_wibeee/compare/v2.2.3...v3.0.0-beta.2) (2021-12-11)


### ⚠ BREAKING CHANGES

* sets `unique_id` on entities, which causes HA to create new entities. Opt out by using `unique_id: false` on the integration.

### Features

* generate entity unique_id from MAC address ([#12](https://github.com/luuuis/hass_wibeee/issues/12)) ([1f8b966](https://github.com/luuuis/hass_wibeee/commit/1f8b966612b3acfb296acde5975fd96d66f3ce9b))
* use human-friendly name for sensors with unique_id, otherwise keep the old name ([#13](https://github.com/luuuis/hass_wibeee/issues/13)) ([bb59ccb](https://github.com/luuuis/hass_wibeee/commit/bb59ccbe518264c336c465ad5fd34521cbac0b12))


### Bug Fixes

* don't update entities that are disabled ([#15](https://github.com/luuuis/hass_wibeee/issues/15)) ([6474db6](https://github.com/luuuis/hass_wibeee/commit/6474db64ae02642b8e40b5df331d093181401b07))

## [3.0.0-beta.1](https://github.com/luuuis/hass_wibeee/compare/v2.2.3...v3.0.0-beta.1) (2021-11-24)


### ⚠ BREAKING CHANGES

* sets `unique_id` on entities, which causes HA to create new entities. Opt out by using `unique_id: false` on the integration.

### Features

* generate entity unique_id from MAC address ([#12](https://github.com/luuuis/hass_wibeee/issues/12)) ([1f8b966](https://github.com/luuuis/hass_wibeee/commit/1f8b966612b3acfb296acde5975fd96d66f3ce9b))
* use human-friendly name for sensors with unique_id, otherwise keep the old name ([#13](https://github.com/luuuis/hass_wibeee/issues/13)) ([bb59ccb](https://github.com/luuuis/hass_wibeee/commit/bb59ccbe518264c336c465ad5fd34521cbac0b12))

## [3.0.0-beta.0](https://github.com/luuuis/hass_wibeee/compare/v2.2.3...v3.0.0-beta.0) (2021-11-22)


### ⚠ BREAKING CHANGES

* sets `unique_id` on entities, which causes HA to create new entities. Opt out by using `unique_id: false` on the integration.

### Features

* generate entity unique_id from MAC address ([#12](https://github.com/luuuis/hass_wibeee/issues/12)) ([1f8b966](https://github.com/luuuis/hass_wibeee/commit/1f8b966612b3acfb296acde5975fd96d66f3ce9b))

### [2.2.3](https://github.com/luuuis/hass_wibeee/compare/v2.2.2...v2.2.3) (2021-08-31)


### Bug Fixes

* make sensors unavailable on status.xml error ([#10](https://github.com/luuuis/hass_wibeee/issues/10)) ([79dc987](https://github.com/luuuis/hass_wibeee/commit/79dc987ec24cfe75d2c254584703e79a82866120))

### [2.2.2](https://github.com/luuuis/hass_wibeee/compare/v2.2.1...v2.2.2) (2021-08-28)


### Bug Fixes

* retry failed requests with exponential backoff ([#9](https://github.com/luuuis/hass_wibeee/issues/9)) ([2fa3e6c](https://github.com/luuuis/hass_wibeee/commit/2fa3e6c3a8c0ca0dc3e395b5cd1b5037949f2acf))

### [2.2.1](https://github.com/luuuis/hass_wibeee/compare/v2.2.0...v2.2.1) (2021-08-25)


### Bug Fixes

* don't error with "Unable to create WibeeeSensor" on unknown keys ([#7](https://github.com/luuuis/hass_wibeee/issues/7)) ([a8d75c3](https://github.com/luuuis/hass_wibeee/commit/a8d75c38cf4b138c065d56187257a58f92ac8559))
* improve error logging to allow bug reports ([#8](https://github.com/luuuis/hass_wibeee/issues/8)) ([3d0297e](https://github.com/luuuis/hass_wibeee/commit/3d0297e969593fd076af3b92aa84b366224b9261))

## [2.2.0](https://github.com/luuuis/hass_wibeee/compare/v2.1.0...v2.2.0) (2021-08-25)


### Features

* add scan_interval support to allow this to be user-configured ([#6](https://github.com/luuuis/hass_wibeee/issues/6)) ([34f4019](https://github.com/luuuis/hass_wibeee/commit/34f401923d389f17f3c8b35ce3b72308a0b26e27))

## [2.1.0](https://github.com/luuuis/hass_wibeee/compare/v2.0.0...v2.1.0) (2021-08-24)


### Features

* Energy support ([#5](https://github.com/luuuis/hass_wibeee/issues/5)) ([113e60e](https://github.com/luuuis/hass_wibeee/commit/113e60ef10666f017c4fdfec54a6dc28ac525bde))


### Bug Fixes

* clean up WibeeeSensor attrs ([#4](https://github.com/luuuis/hass_wibeee/issues/4)) ([4859014](https://github.com/luuuis/hass_wibeee/commit/485901464706fbe2b2b0d52839364d6a924e7d23))

### [2.0.1](https://github.com/luuuis/hass_wibeee/compare/v2.0.0...v2.0.1) (2021-08-22)


### Bug Fixes

* removes WibeeeSensor `icon` and `unique_id` ([5230596](https://github.com/luuuis/hass_wibeee/commit/5230596b14277f7df5932fb9ca3c3e28552284a0))

## 2.0.0 (2021-08-22)


### Bug Fixes

* specify `iot_class` for custom component, add hassfest workflow ([#1](https://github.com/luuuis/hass_wibeee/issues/1)) ([6a5c9c8](https://github.com/luuuis/hass_wibeee/commit/6a5c9c86c104bb32ccb7fff3da0086fc898b4446))
