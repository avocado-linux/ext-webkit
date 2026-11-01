# Changelog

All notable changes to avocado-ext-webkit are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.1]

### Fixed
- `supported_targets` lists every machine whose feed builds `wpewebkit`: all
  declared machines except the two qemus. The old list was partial, named the
  pre-rename Jetson `-devkit` targets the 2024 feed dropped, and named
  `icam-540`, a BSP rather than a feed machine.
- `test.yml` gains the 2026 leg, matching `release.yml`.

## [0.1.0]

### Added
- Initial release: WPE WebKit browser and display utilities.
- CI via the shared `avocado-linux/actions` reusable workflows: PR build check
  (`test.yml`) and tag-driven package + publish to the Avocado feed (`release.yml`).
