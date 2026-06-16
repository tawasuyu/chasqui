# chasqui

> Sovereign peer discovery + transport — DHT, relay, NAT traversal — in Rust.

`chasqui` (Quechua: *Inca relay messenger*) is the networking layer: peer discovery (UDP + Kademlia DHT), relay/dcutr/autonat for NAT traversal, and authenticated transport over the `card` identity. Channels and capabilities are expressed as typed cards; no TCP/IP assumptions leak into the apps above it.

<p align="center">
  <img src="docs/chasqui_showreel.gif" alt="chasqui showreel — the broker explorer: health state, active sessions with their in/out flows, and a live timeline of peer matches" width="900">
  <br>
  <sub>the broker's live monitor — health, active sessions &amp; flows, and the peer-match timeline</sub>
</p>

## How dependencies work
Front-door repo: only `chasqui-*` crates here. `card` (identity), `arje` primitives, shared leaves are git-dependencies of the [`tawasuyu`](https://github.com/tawasuyu/tawasuyu) monorepo.

## License
MIT. Part of the [tawasuyu](https://github.com/tawasuyu/tawasuyu) suite.
