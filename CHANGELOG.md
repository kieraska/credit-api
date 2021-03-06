# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.4.7] - 16-02-2021

### Changed
- Added missing `insurance` field in the simulation update

## [1.4.6] - 14-02-2021

### Changed
- General refactor in some classes
- Data changed in the `LoadDatabase` class
- `spring-boot-starter-parent` version update

## [1.4.5] - 06-02-2021

### Changed
- Renamed the Simulation advice
- Added generic exception for Simulation not found by name

### Removed
- Custom exception for Simulation not found by name

## [1.4.4] - 06-02-2021

### Changed
- Bump version due to the GitHub Actions conflict with the previous version

## [1.4.3] - 06-02-2021

### Changed
- Renamed all the classes replacing Simulator by Simulation
- Changed the Api response example for the GET and PUT endpoints on SimulationController  

## [1.4.2] - 05-02-2021

### Added
- Added `system.properties` file to enable the Heroku deploy

## [1.4.1] - 05-02-2021

### Added
- Added `spring.profiles.active=default`

### Changed
- Updated lombok dependency to `1.18.18`
- Updated `README` with the two different ways to change the port

## [1.4.0] - 31-01-2021

### Changed
- Changed the log levels to remove the console logger verbosity 

## [1.3.0] - 31-01-2021

### Added
- GitHub workflow
- Added configuration for swagger on `application.properties`
- Added `springfox-swagger2` library
- Added `ApiParam` description for the `GET` mappings on `RestrictionController`

### Changed
- Updated the following library versions
    - spring-boot-starter-parent-2.4.1
    - springfox-3.0.0
    - maven.compiler.plugin-3.8.1
    - maven-failsafe.version>3.0.0-M5
  
### Removed
- Removed `SneakyThrows` on `SimulatorController`
- Removed `@Swagger2` annotation on `SwaggerConfig`
- Renamed the main class to `Run`