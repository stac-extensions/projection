# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [v2.0.0] - 2024-07-22

### Removed

- The formerly deprecated field `proj:espg` was removed in favor of `proj:code`.
  A former `"proj:epsg": 3857` is now `"proj:code": "EPSG:3857"`.

## [v1.2.0] - 2024-07-22

### Added

- The new field `proj:code` was introduced as a more general way to describe projection codes for various authorities, not just EPSG.

### Changed

- Updated PROJJSON schema version from 0.5 to 0.7

### Deprecated

- `proj:espg` was deprecated in favor of `proj:code`.
  A former `"proj:epsg": 3857` is now `"proj:code": "EPSG:3857"`.

## [v1.1.0] - 2023-02-10

### Added

- Added examples for Collections and Assets (in Items)

### Changed
- `proj:epsg` is not required in Item properties anymore. `proj:epsg` is recommended now, but not required in any scope.
- Updated the PROJJSON schema to v0.5

### Fixed

- Added missing scope "Collection" to Readme. The scope was already supported in JSON Schemas.
- Clarify that `proj:wkt2` or `proj:projjson` should be used for complex (non-EPSG) CRS
- Clarified which fields are required by GDAL
- Recommendation for thumbnails

## [v1.0.0] - 2021-03-30

Initial independent release, see [previous history](https://github.com/radiantearth/stac-spec/commits/v1.0.0-rc.2/extensions/projection)

[Unreleased]: <https://github.com/stac-extensions/projection/compare/v2.0.0...HEAD>
[v2.0.0]: <https://github.com/stac-extensions/projection/compare/v1.2.0...v2.0.0>
[v1.2.0]: <https://github.com/stac-extensions/projection/compare/v1.1.0...v1.2.0>
[v1.1.0]: <https://github.com/stac-extensions/projection/compare/v1.0.0...v1.1.0>
[v1.0.0]: <https://github.com/stac-extensions/projection/tree/v1.0.0>
