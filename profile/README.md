# 🍰 PixelCake

**Infrastructure, piece by piece.**

PixelCake is a browser-based designer for small networks. You draw the network, then you ask it a question:
does this PC reach that server? If it does not, you see where the traffic stops and why.

What the prototype does today:

- **Draw**: devices, links, VLANs, ports and network cards on an interactive canvas, with auto-layout and several boards per project
- **Test**: ping, web, download and email flows are checked hop by hop with basic rules (physical path, VLAN membership, subnets, gateways) and animated on the drawing
- **Type**: a built-in terminal with a small vendor-neutral command language (`ping`, `trace`, `show`, `set`, `connect`)
- **Export**: the topology as YAML, which can be loaded back; a Terraform-style export exists only as a sketch

What it does not do: it is not a packet-level simulator (no ARP, routing tables, spanning tree or NAT),
and it cannot read existing Terraform state.

**Status:** early prototype, still in the oven. The code stays private while it bakes.

Built by [@Phil-pje](https://github.com/Phil-pje) with React, TypeScript and React Flow.
