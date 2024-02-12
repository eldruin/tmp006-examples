# Archived. See [driver-examples](https://github.com/eldruin/driver-examples)

## Additional example programs for the [tmp006] crate [![Build Status](https://travis-ci.org/eldruin/tmp006-examples.svg?branch=master)](https://travis-ci.org/eldruin/tmp006-examples)

[tmp006]: https://crates.io/crates/tmp006

This repository contains additional example programs using the TMP006 I2C non-contact infrared
(IR) thermopile temperature sensor with an STM32F3Discovery board.

These examples expect that you connect the TMP006 device to the pins PB6 (SCL)
and PB7 (SDA) of the discovery board.

For example, to run the f3-display example:
First, connect your discovery board per USB, then connect OpenOCD in a terminal with:
```
openocd -f interface/stlink-v2-1.cfg -f target/stm32f3x.cfg
```

Then on another terminal run:
```
git clone https://github.com/eldruin/tmp006-examples
cd tmp006-examples
cargo run --example f3-display
```

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

