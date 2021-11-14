[![CI](https://github.com/lpenz/yacopstr/actions/workflows/ci.yml/badge.svg)](https://github.com/lpenz/yacopstr/actions/workflows/ci.yml)
[![coveralls](https://coveralls.io/repos/github/lpenz/yacopstr/badge.svg?branch=main)](https://coveralls.io/github/lpenz/yacopstr?branch=main)
[![crates.io](https://img.shields.io/crates/v/yacopstr)](https://crates.io/crates/yacopstr)
[![doc.rs](https://docs.rs/yacopstr/badge.svg)](https://docs.rs/yacopstr)


# yacopstr: Yet Another COPy STRing module

yacopstr's [`Str`] wraps a fixed-size array of `u8` and provides a
string-like interface on top. The size is specified using a const
generic argument.

The internal `u8` array corresponds to UTF-8 encoded `chars`. All
functions guarantee that the contents are valid UTF-8 and return
an error if they are not.

[`Str`]: https://docs.rs/yacopstr/0/yacopstr/struct.Str.html
