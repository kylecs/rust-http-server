# Rust HTTP Static
A static file HTTP/1.1 server written in rust. This server aims to be compliant
with HTTP/1.1, however some requirements are still missing.

# Using
Download the project:

`git clone https://github.com/kylecs/Rust-HTTP-Static.git`

Build with cargo:

`cargo build --release`

Run:

`sudo ./target/release/rust-http-static -d *directory*`

## Supports
* GET and HEAD requests
* Persistent Connections
* Requires host header
* 100 Continue response
* Date response header

## Does not support
* Chunked Transfer-Encoding (Do I really need this without supporting POST requests?)
* If-Modified-Since and If-Unmodified-Since headers

## Why
My primary goal with this project was to familiarize myself with both rust
and the HTTP/1.1 protocol. This is only meant to be a novelty and is
sure to be riddled with spec violations and security vulnerabilities.
