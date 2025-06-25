# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed
- Updated Java version from 21 to 24. (Source: `pom.xml`, `git` commit `684ee40`)
- Updated Spring Boot version to `3.5.3`. (Source: `pom.xml`)
- Updated Spring Cloud version to `2025.0.0`. (Source: `pom.xml`)
- Updated OpenTelemetry version to `2.16.0`. (Source: `pom.xml`)
- Updated project dependencies and documentation. (Source: `git` commit `c2252e2`)
- Added Caffeine cache dependency. (Source: `pom.xml`)
- Added OpenTelemetry Spring Boot Starter. (Source: `pom.xml`)

### Added
- Health check endpoint. (Source: `git` commit `9a43bca`)
- CI badge to `README.md`. (Source: `git` commit `4ee7a3b`)
- Spring Boot Actuator for health monitoring and metrics. (Source: `pom.xml`)
- Spring Cloud Bootstrap for additional configuration options. (Source: `pom.xml`)

## [0.0.1] - 2024-03-23

### Added
- Initial release
- Basic Eureka Server implementation
- Docker support
- GitHub Actions CI/CD pipeline