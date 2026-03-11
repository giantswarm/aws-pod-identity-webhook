# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed

- Add `io.giantswarm.application.audience: all` annotation to publish the app to the customer Backstage catalog.
- Migrate chart metadata annotations to `io.giantswarm.application.*` format.

## [2.2.0] - 2026-02-24

### Changed

- Sanitize `Chart.Version` when used in labels due to flux appending the artifact digest to the version.

## [2.1.0] - 2025-12-01

### Changed

- Set VPA `minAllowed` CPU to 50m. Otherwise VPA will set the CPU to tiny values that will cause CPU throttling.

## [2.0.0] - 2025-10-21

### Changed

- Upgrade IRSA to latest v0.6.9

[Unreleased]: https://github.com/giantswarm/aws-pod-identity-webhook/compare/v2.2.0...HEAD
[2.2.0]: https://github.com/giantswarm/aws-pod-identity-webhook/compare/v2.1.0...v2.2.0
[2.1.0]: https://github.com/giantswarm/aws-pod-identity-webhook/compare/v2.0.0...v2.1.0
[2.0.0]: https://github.com/giantswarm/aws-pod-identity-webhook/compare/v1.19.1...v2.0.0
