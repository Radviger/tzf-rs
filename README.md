# WIP: tzf's Rust port. [![Rust](https://github.com/ringsaturn/tzf-rs/actions/workflows/rust.yml/badge.svg)](https://github.com/ringsaturn/tzf-rs/actions/workflows/rust.yml)

## Usage

Add to `Cargo.toml`

```toml
tzf-rs = { git =  "http://github.com/ringsaturn/tzf-rs", rev = "868b272159d9cea3c2cd2d8d36a40080de6a9e83"}
```

NOTE: This package is still working in process and `868b272159d9cea3c2cd2d8d36a40080de6a9e83`
is the latest stable commit for now.

```rust
use std::time::Instant;
use tzf_rs::Finder;

fn main() {
    let finder = Finder::new();

    print!("{:?}\n", finder.get_tz_name(116.3883, 39.9289));
}
```

## References:

- Original Go repo: <https://github.com/ringsaturn/tzf>
- Binary timezone data: <https://github.com/ringsaturn/tzf-rel>
- Geometry: <https://github.com/ringsaturn/geometry-rs>
  which is <https://github.com/tidwall/geometry>'s Rust port.
