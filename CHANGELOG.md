# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2021-01-30

### Changed

- Changed Signals into using signed 16-bit integers per the specification. This change makes it API breaking.

### Fixed

- Temperature and humidity words were swapped and now this actually reports correctly. Be careful with 200 multiplier with temperature as it fooled me once.
- Changing more unsigned to signed helps to detect negative temperatures :-)


## [0.0.2] - 2021-01-12

### Changed

- set_voc_states
- get_voc_states
- store_input_parameters
- get_voc_parameters
- set_voc_parameters

Improved the documentation and validating that get_temperature_offset works after upgrading
the device firmware into 2.2.


## 0.0.1 - 2021-01-11

Initial release to crates.io. The crate moves into 0.1.x versioning after embedded-hal change.

[1.0.0]: https://github.com/mjaakkol/svm40-rs/compare/v0.0.2...v1.0.0

[0.0.2]: https://github.com/mjaakkol/svm40-rs/compare/v0.0.1...v0.0.2

[i5]: https://github.com/mjaakkol/svm40-rs/pull/5
