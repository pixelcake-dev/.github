<p>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/pixelcake-dev/.github/main/profile/assets/pixelcake-orizzontale-negativo.svg">
    <img src="https://raw.githubusercontent.com/pixelcake-dev/.github/main/profile/assets/pixelcake-orizzontale-colore.svg" alt="PixelCake" width="300">
  </picture>
</p>

**Infrastructure, piece by piece.**

PixelCake is a visual designer for small networks that runs in the browser. You draw the network, configure it for real,
then ask it a question: does this PC reach that server? If it does not, you see where the packet stops, and why.

One place to do three things with a network:

- **Design**: devices, links, ports and network cards on a canvas, with their addresses, VLANs, static routes, firewall zones and ordered rules, NAT and port forwards
- **Ask**: ping, web, download and email flows are followed hop by hop, from a panel or from a built-in terminal with a small vendor-neutral command language; when a flow fails, the answer names the device that stopped it, and the port, the route or the rule it used
- **Present**: a presentation mode to ask questions on the drawing, break a cable or a device and see what stops working; the board goes out as a picture, PNG or SVG

What it does not do: it does not go down to single frames (no ARP, no MAC tables), its routes are static,
and there is no DHCP, DNS or spanning tree yet. The topology exports to YAML and loads back; the Terraform export is only a sketch.

**Status:** early prototype. The code stays private until it is ready.

Built by [@Phil-pje](https://github.com/Phil-pje) with React, TypeScript and React Flow.
