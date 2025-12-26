# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/).

## [0.5.8] - 2025-12-26

### Added
- GitHub Actions release workflow gated on tests that:
  - builds and attaches `sdist`/`wheel` artifacts to a GitHub Release
  - publishes the `crossplane-ng` distribution to PyPI
  - builds and pushes a multi-arch Docker image running the `crossplane` CLI

### Changed
- PyPI distribution name is now `crossplane-ng` (import and CLI remain `crossplane`).
- Packaging no longer imports `crossplane` during builds to avoid import-time side effects.


