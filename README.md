# Rust Template

## Configure this template

Change the the project name by modifying the name key in [Cargo.toml](Cargo.toml). Make sure you also modify the new name in the BINARY & RELEASE variables found in [cd.yml](.github/workflows/cd.yml).

```bash
# To enable client side git hooks
git config core.hooksPath hooks/
```
## GitHub Actions used in this template

- GitHub Checkout - [actions/checkout@v3](https://github.com/actions/checkout)
- Rust Toolchain - [actions-rs/toolchain@v1](https://github.com/actions-rs/toolchain)
- Cargo - [actions-rs/cargo@v1](https://github.com/actions-rs/cargo)
- GitHub Release - [softprops/action-gh-release@v1](https://github.com/softprops/action-gh-release)

For more Rust related GitHub Actions visit [actions-rs](https://github.com/actions-rs)

## Replace with new project

```bash
# Delete current default cargo project
rm -rf target src Cargo.toml Cargo.lock
```

```bash
# Use this command to initialize you're very own rust project
cargo init --name <NAME_OF_PACKAGE>
```

```bash
# Check out other possible options
cargo init --help
```