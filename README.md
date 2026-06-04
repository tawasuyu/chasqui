# chasqui

> Sovereign peer discovery + transport — DHT, relay, NAT traversal — in Rust.

`chasqui` (Quechua: *Inca relay messenger*) is the networking layer: peer discovery (UDP + Kademlia DHT), relay/dcutr/autonat for NAT traversal, and authenticated transport over the `card` identity. Channels and capabilities are expressed as typed cards; no TCP/IP assumptions leak into the apps above it.

## How dependencies work
Front-door repo: only `chasqui-*` crates here. `card` (identity), `arje` primitives, shared leaves are git-dependencies of the [`gioser`](https://gitea.gioser.net/sergio/gioser) monorepo.

## License
MIT. Part of the [gioser](https://gitea.gioser.net/sergio/gioser) suite.
