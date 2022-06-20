# rust template repository

## Configure this template

Change the the project name by modifying the name key in [Cargo.toml](Cargo.toml). Make sure you also modify the new name in the BINARY & RELEASE variables foung in [Continuous Delivery](.github/workflows/cd.yml).

```bash
# To enable client side git hooks
git config core.hooksPath hooks/
```

## Create new project from scratch

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