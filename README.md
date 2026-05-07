# asdf-rust

[Rust](https://www.rust-lang.org) plugin for asdf version manager

## Build History

[![Build history](https://buildstats.info/github/chart/asdf-community/asdf-rust?branch=master)](https://github.com/asdf-community/asdf-rust/actions)

## Installation

```bash
asdf plugin add rust https://github.com/asdf-community/asdf-rust.git
```

## Usage

Check the [asdf](https://github.com/asdf-vm/asdf) readme for instructions on
how to install & manage versions.

## Configuration

By default, `asdf-rust` installs rust via
[Standalone installers](https://forge.rust-lang.org/infra/other-installation-methods.html)
with all included components.

That includes the docs, which may easily be around ~50% of the total install size.
For this reason there is a `RUST_WITHOUT` environment variable, which takes a
comma-separated list of components NOT to install:

```sh
RUST_WITHOUT=rust-docs,rust-other-component asdf install rust 1.95.0

# Or in .profile
export RUST_WITHOUT=rust-docs
```

## License

Licensed under the
[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
