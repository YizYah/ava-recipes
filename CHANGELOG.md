# Change Log

All notable changes to the "ava-recipes" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [1.0.0] - 2021-08-26

### Added

- learning notes

## [1.0.1] - 2021-08-26

### Fixed

- updated the `test-no-content` key to have a different value than that for `test`, because it had overwritten it.

## [1.0.2] - 2021-08-26

### Added

- better README documentation

## [1.0.3] - 2021-09-09

### Added

- added javascript capability

## [1.0.4] - 2021-09-09

### Added

- added `throws-expect-async`. Will save a lot of frustration caused by a missing `await` somewhere.

## [1.0.5] - 2021-09-12

### Fixed

- fixed `step`. It had two tab stops with the same number.

## [1.0.6] - 2021-09-14

### Added

- `stub` and `learn-stub` now generate comments explaining where to insert imports for code that uses the stub.

## [1.0.7] - 2021-09-29

### Added

- `stub` and `learn-stub` now use rewire.

## [1.0.8] - 2021-10-03

### Updated

- `stub` and `stub-private` updated to `stub-constant` and `stub-module` and refactored.
- `test...` snippets changed to `new...` to distinguish from the several `test...` snippets in the popular `AVA` package.  Also created an async version.
