# Avail Rehber

# Gereksinimler

* 2 CPU
* 4GB RAM
* 20-40GB SSD
* Ubuntu 20.04 ya da üstü

# Kurulum

Sistemi güncelleyelim.

```
sudo apt update && sudo apt upgrade -y
```
Gerekli paketleri yükleyelim.

```
sudo apt install make clang pkg-config libssl-dev build-essential git screen protobuf-compiler -y
```
Rust kuralım ve ayarlayalım.

```
curl https://sh.rustup.rs -sSf | sh
source $HOME/.cargo/env
rustup update nightly
rustup target add wasm32-unknown-unknown --toolchain nightly
```
