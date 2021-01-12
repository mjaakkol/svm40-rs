# svm40-rs
Platform agnostic Rust device driver for Sensirion SVM40 development board

[![Build status][workflow-badge]][workflow]
[![Crates.io Version][crates-io-badge]][crates-io]
[![Crates.io Downloads][crates-io-download-badge]][crates-io-download]
![No Std][no-std-badge]

Platform agnostic Rust driver for Sensirion SVM40 device with gas, temperature and humidity sensors 
based on the [`embedded-hal`](https://github.com/japaric/embedded-hal) traits.

## Sensirion SVM40

Sensirion SVM40 has 2nd generation low-power accurate SGP40 gas sensor for air quality application 
and SHT40 sensor measuring temperature and humidity. The sensor uses I²C interface and measures 
VOC (*Total Volatile Organic Compounds*)

Evaluation board: https://www.sensirion.com/cn/environmental-sensors/evaluation-kit-sek-svm40/

## Development status
The sensor supports starting and stopping measurement as well as gathering the values but
there are still work to do:
- Improve documentation
- Moving into using Embedded-hal 1.x
- Improve crate module tests
- Maybe add async support (most waits are so short that it might not make sense)
- Add VOC states management
- Add VOC parameters management
- Implement storing of input parameters


## License

Licensed under either of

 * Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
   http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or
   http://opensource.org/licenses/MIT) at your option.


### Contributing

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.

<!-- Badges -->
[workflow]: https://github.com/mjaakkol/svm40-rs/actions?query=workflow%3ARust
[workflow-badge]: https://img.shields.io/github/workflow/status/mjaakkol/svm40-rs/Rust/master
[crates-io]: https://crates.io/crates/svm40
[crates-io-badge]: https://img.shields.io/crates/v/svm40.svg?maxAge=3600
[crates-io-download]: https://crates.io/crates/svm40
[crates-io-download-badge]: https://img.shields.io/crates/d/svm40.svg?maxAge=3600
[no-std-badge]: https://img.shields.io/badge/no__std-yes-blue
