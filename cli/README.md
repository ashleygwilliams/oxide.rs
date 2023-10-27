# The Oxide CLI

## Installation

#### Pre-built binaries
We offer pre-built binaries for Intel Mac, Mac Silicon, Windows, Linux-glibc, and Linux-musl. You can download them and manually add them to your path or you can use one of several installation options we offer. Checkout [link to website?](?) or our [Github Releases](https://github.com/oxidecomputer/oxide.rs/releases) to get started.

#### From source
Build with `cargo build --bin oxide` and add the executable in `target/debug` to your `PATH`.

## Authentication

There are two ways to authenticate against the Oxide rack using the CLI:

- Environment variables: You can set the `OXIDE_HOST` and `OXIDE_TOKEN` environment variables. This method is useful for service accounts.

- Configuration file: When running the `oxide auth login` command, a `$HOME/.config/oxide/hosts.toml` file is generated. This file contains sensitive information like your token and user ID.
