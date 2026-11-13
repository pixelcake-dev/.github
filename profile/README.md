# 🍰 PixelCake

**Infrastructure, piece by piece.**

PixelCake is a browser-based designer for small networks. You draw the network, configure it, then you ask it a question:
does this PC reach that server? If it does not, you see where the traffic stops and why.

What it does today:

- **Draw**: devices, links, ports and network cards on an interactive canvas, with auto-layout and several boards per project
- **Configure**: addresses, VLANs port by port, static routes, firewall zones and ordered rules, NAT and port forwards
- **Test**: ping, web, download and email flows are followed hop by hop and animated on the drawing; when one fails, the reason names the port, the route or the rule
- **Type**: a built-in terminal with a small vendor-neutral command language (`ping`, `trace`, `browse`, `show routes`, `add rule` and more)
- **Present**: a presentation mode to ask questions on the drawing, break a cable or a device and see what stops working; the board goes out as a picture, PNG or SVG
- **Export**: the topology as YAML, which can be loaded back; a Terraform-style export exists only as a sketch

What it does not do: it does not go down to single frames (no ARP, no MAC tables), its routes are static,
and there is no DHCP, DNS or spanning tree yet. It cannot read existing Terraform state.

**Status:** early prototype, still in the oven. The code stays private while it bakes.

Built by [@Phil-pje](https://github.com/Phil-pje) with React, TypeScript and React Flow.
