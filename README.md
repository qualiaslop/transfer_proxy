# transfer_proxy

An asynchronous Minecraft "proxy" that forwards connections to different servers via the hostname, including support for the new transfer packets in modern versions to minimise network load.

## Features

- **Minecraft protocol handling:** Processes handshake, login and status packets before routing to the correct recipient server
- **Proxy fallback:** When transfer protocol is unavailable, the server falls back to a bidirectional TCP proxy.
- **Protocol compatibility:** Supports connections across different Minecraft protocol versions. Supports the HAProxy TCP protocol
- **Nix integration:** Includes a NixOS module for declarative deployment and service configuration.


## Technology

Built with **Rust** and the **Tokio** async framework

