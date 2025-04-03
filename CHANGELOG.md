# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed
- Updated Java version from 21 to 24
- Updated Spring Boot version from 3.4.0 to 3.4.4
- Updated Spring Cloud version from 2024.0.0 to 2024.0.1
- Updated Docker base images to use Java 24:
  - Changed `eclipse-temurin:21-jre-alpine` to `eclipse-temurin:24-jre-alpine`
  - Changed `maven:3-eclipse-temurin-21-alpine` to `maven:3-eclipse-temurin-24-alpine`
- Updated GitHub Actions workflow to use Java 24

## [0.0.1] - 2024-03-23

### Added
- Initial release
- Basic Eureka Server implementation
- Docker support
- GitHub Actions CI/CD pipeline 