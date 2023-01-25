# Testing cross-compile problems found with openssl-sys

Requirements: docker

```bash
cargo install cross
```

```bash
rustup target list
```

```bash
rustup target add aarch64-unknown-linux-gnu
```

```bash
cross build --workspace --locked --target aarch64-unknown-linux-gnu
```

```bash
cargo build --workspace --locked --target aarch64-unknown-linux-gnu
```
