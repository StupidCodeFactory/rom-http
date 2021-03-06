# v0.7.0 2018-01-11

### Added
  - Add Dataset#add_params(AMHOL)

### Changed
  - Updated error messages (AMHOL)
  - updated to depend on ROM 4.0 (maximderbin)
  - Removed ruby 2.1 support (maximderbin)
  - Removed rbx-3 support (maximderbin)



[Compare v0.5.0...v0.6.0](https://github.com/rom-rb/rom-http/compare/v0.6.0...v0.7.0)

# v0.6.0 2017-02-06
### Changed
  - Make schemas mandatory and use schema API from ROM core (AMHOL)
  - Generate transformer using schema (AMHOL)
  - Removed rbx-2 support (solnic)
  - Add Dataset#base_path and Relation#primary_key (AMHOL)
  - Updated to work with ROM 3.0 (maximderbin)
  - Removed ruby 2.1 support (maximderbin)
  - Fix Relation#primary_key when schema defines alias (AMHOL)
  - Transform keys on insert and update (maximderbin)
  - Remove `rom-support` dependency (maximderbin)

[Compare v0.5.0...v0.6.0](https://github.com/rom-rb/rom-http/compare/v0.5.0...v0.6.0)

# v0.5.0 2016-08-08
### Changed
  - Removed ruby 2.0 support
  - Use `schema` API from ROM::Core.  Replaces old schema (solnic)
  - Now works out of the box with `rom-repository` (solnic)

[Compare v0.4.0...v0.5.0](https://github.com/rom-rb/rom-http/compare/v0.4.0...v0.5.0)

# v0.4.0 2016-04-30
### Changed
  - updated to depend on the forthcoming rom 2.0 (cflipse)

[Compare v0.3.0...v0.4.0](https://github.com/rom-rb/rom-http/compare/v0.3.0...v0.4.0)

# v0.3.0 2016-03-17

### Changed
  - replaced dry-data with dry-types  (Nikita Shilnikov <ns@latera.ru>)

[Compare v0.2.0...v0.3.0](https://github.com/rom-rb/rom-http/compare/v0.2.0...v0.3.0)

# v0.2.0 2016-01-30
### Added

  - schema support using `dry-data` (AMHOL)

[Compare v0.1.2...v0.2.0](https://github.com/rom-rb/rom-http/compare/v0.1.2...v0.2.0)

# v0.1.2 2015-09-16
### Added

  - Projections (`container.relation(:users).project(:id, :name)`) (AMHOL)

[Compare v0.1.1...v0.1.2](https://github.com/rom-rb/rom-http/compare/v0.1.1...v0.1.2)

# v0.1.1 2015-09-03
### Added

  - `ROM::HTTP::Dataset` macros for setting `default_request_handler` and `default_response_handler` (AMHOL)

### Changed

- `ROM::HTTP::Gateway` tries to load the `Dataset` class lazily from the same namespace that the `Gateway` is defined in, with a fallback to `ROM::HTTP::Dataset`, making extending easier (AMHOL)
- `ROM::HTTP::Gateway` no longer raises errors on missing configuration keys, these are now raised late in `Dataset` - this was to allow for the implementation of `default_request_handler` and `default_response_handler` (AMHOL)
- `ROM::HTTP::Dataset` now uses `ROM::Options` from `rom-support`, adding typechecking to options and making it easier to define additional options in extensions

[Compare v0.1.0...v0.1.1](https://github.com/rom-rb/rom-http/compare/v0.1.0...v0.1.1)

# v0.1.0 2015-08-19

First public release \o/
