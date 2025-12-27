# Bevy WebGL project Template

This is the template for bevy project for WebGL.

## Setup

You need rustup to build wasm and also wasm-bindgen to get JS bindings.

Installing rust up

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Add rust wasm target and wasm-bindgen
```
rustup target add wasm32-unknown-unknown
cargo install wasm-bindgen-cli
```
You need to add cargo binaries to the path 

For Fish
```
set -Ux PATH $HOME/.cargo/bin $PATH
```
I am using Task as build system. [go-task](https://taskfile.dev/)


## Usage

Build the project for dev
```
task build-dev
```

Build the project for release
```
task build-release
```
Run the server
```
task serve
```
It will be hosted in localhost:8000



