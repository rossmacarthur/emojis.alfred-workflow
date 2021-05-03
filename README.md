# emojis.alfredworkflow

[![Build status](https://github.com/rossmacarthur/emojis.alfredworkflow/actions/workflows/build.yaml/badge.svg)](https://github.com/rossmacarthur/emojis.alfredworkflow/actions/workflows/build.yaml)

Alfred workflow to fuzzy search emojis and copy them to clipboard.

## Features

- Fuzzy search based on description and GitHub shortcodes / aliases.
- Uses the latest Unicode emoji spec (v13.1).
- Blazingly fast 🤸 (it's built in Rust).

## 📦 Installation

### Pre-packaged

Grab the latest release from
[the releases page](https://github.com/rossmacarthur/emojis.alfredworkflow/releases).

Because the release contains an executable binary later versions of macOS will
mark it as untrusted and Alfred won't be able to execute it. You can run the
following to explicitly trust the release before installing to Alfred.
```sh
xattr -c ~/Downloads/emojis-*-x86_64-apple-darwin.alfredworkflow
```

### Building from source

This workflow is written in Rust, so to install it from source you will first
need to install Rust and Cargo using [rustup](https://rustup.rs/). Then install
[powerpack](https://github.com/rossmacarthur/powerpack). Then you can run the
following to build an `.alfredworkflow` file.

```sh
git clone https://github.com/rossmacarthur/emojis.alfredworkflow.git
cd emojis.alfredworkflow
powerpack package
```

The release will be available at `target/workflow/emojis.alfredworkflow`.

## License

Licensed under either of

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
  http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.
