# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed
- Updated Java version from 21 to 24. (Source: `pom.xml`, `git` commit `684ee40`, `Dockerfile`, `.github/workflows/maven.yml`)
- Updated Spring Boot version to `3.5.0`. (Source: `pom.xml`)
- Updated Spring Cloud version to `2025.0.0`. (Source: `pom.xml`)
- Updated Docker base images to use Java 24: (Source: `Dockerfile`, `Dockerfile.local`)
  - `eclipse-temurin:24-jre-alpine`
  - `maven:3-eclipse-temurin-24-alpine`
- Updated GitHub Actions workflow to use Java 24. (Source: `.github/workflows/maven.yml`)

### Added
- Health check endpoint. (Source: `git` commit `9a43bca`)
- CI badge to `README.md`. (Source: `git` commit `4ee7a3b`)

## [0.0.1] - 2024-03-23

### Added
- Initial release
- Basic Eureka Server implementation
- Docker support
- GitHub Actions CI/CD pipeline