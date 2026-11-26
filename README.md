# Awesome-Network-Routing-Traffic-Aggregation

# Awesome-Network-Routing-Traffic-Aggregation

## Top Network Routing & Traffic Aggregation Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on SD-WAN, Traffic Aggregation, Multi-Link Bonding & Network Optimization*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Network Routing & Traffic Aggregation**. These tools intelligently route, bond, and optimize network traffic across multiple WAN links, replacing traditional MPLS with secure, software-defined connectivity.

**Examples** include Cloudflare Magic WAN, Cisco Meraki, Fortinet Secure SD-WAN, Palo Alto Prisma SD-WAN, Aruba EdgeConnect, VMware SD-WAN, Cato Networks, Cradlepoint, Versa Networks, Aryaka, and rohit267/net-merge (the category leaders and notable projects).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, multi-link bonding, and traffic aggregation — ideal for homelabs, SMBs, and developers building transparent network solutions without vendor lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Cloudflare Magic WAN](https://developers.cloudflare.com/cloudflare-wan/)**  
  Cloud-native WAN-as-a-Service connecting sites via IPsec/GRE tunnels to Cloudflare's global network, replacing MPLS with inline security at the edge [citation:1].

- **[Cisco Meraki SD-WAN](https://www.cisco.com/)**  
  Cloud-managed SD-WAN with Auto VPN, active/active paths, and integrated security (IDS/IPS, AMP) on MX appliances [citation:2].

- **[Fortinet Secure SD-WAN](https://www.fortinet.com/products/sd-wan)**  
  Converged networking and security on FortiOS, with SD-WAN, ZTNA, and SSE managed from a single pane [citation:3].

- **[Palo Alto Prisma SD-WAN](https://docs.paloaltonetworks.com/prisma-sd-wan)**  
  App-defined autonomous SD-WAN as part of Prisma SASE, with AI-powered Strata Cloud Manager for unified management [citation:4].

- **[HPE Aruba EdgeConnect SD-WAN](https://www.hpe.com/)**  
  Business-intent overlay with path conditioning, WAN optimization, and tight integration into HPE's SASE platform [citation:5].

- **[VMware SD-WAN (VeloCloud)](https://www.vmware.com/products/sd-wan.html)**  
  Cloud-delivered SD-WAN with Dynamic Multi-Path Optimization (DMPO) and optional single or dual-vendor SASE [citation:6].

- **[Cato Networks](https://www.catonetworks.com/)**  
  Converged SD-WAN and security on a global private backbone with 65+ PoPs, delivered as a cloud-native SASE platform [citation:7].

- **[Ericsson Cradlepoint](https://cradlepoint.com/)**  
  Cellular-first SD-WAN and wireless WAN solutions managed via NetCloud, strong in retail, transport, and public safety [citation:8].

- **[Versa Networks](https://versa-networks.com/)**  
  Multi-tenant, cloud-native Secure Cloud IP platform unifying SD-WAN, SD-Security, and SD-Branch in one software stack [citation:9].

- **[Aryaka](https://www.aryaka.com/)**  
  Fully managed SD-WAN built on a global private backbone, with integrated security and 24/7 support included [citation:10].

- **[rohit267/net-merge](https://github.com/rohit267/net-merge)**  
  System-wide per-connection traffic balancing across Wi-Fi, Ethernet, and tethers on Windows, macOS, and Linux [citation:11][citation:21].

## Open-Source GitHub Projects

- **[net-merge](https://github.com/rohit267/net-merge)**  
  System-wide per-connection balancing that pins each TCP/UDP connection to a specific adapter, spreading load across Wi-Fi, Ethernet, and USB tethers with automatic adapter detection and per-adapter health checks [citation:11][citation:21].

- **[OpenMPTCProuter](https://github.com/Ycarus/OpenMPTCProuter)**  
  OpenWrt-based firmware that aggregates multiple internet connections (DSL, fiber, 4G/5G) at the packet level using Multipath TCP, merging links into a single encrypted stream [citation:25].

- **[vtrunkd](https://github.com/VrayoSystems/vtrunkd)**  
  Open-source SD-WAN daemon for Linux providing network link bonding, trunking, and aggregation with multichannel VPN capabilities [citation:24][citation:28].

- **[PolyWAN](https://crates.io/crates/polywan)**  
  Multi-WAN routing and failover daemon for Linux, spreading new connections over multiple uplinks with health checks, sticky connections, and nftables integration [citation:20].

- **[tailbond](https://github.com/kaovilai/tailbond)**  
  Speedify-style WAN bonding (Wi-Fi + 5G + Ethernet) to a home server or VPS, with Tailscale integration and support for OpenWrt routers, Fedora, and containers [citation:19].

- **[NovaEdge](https://github.com/azrtydxb/novaedge)**  
  Kubernetes-native SD-WAN and service mesh with multi-link WAN management, application-aware path selection, WireGuard tunnels, and real-time link quality probing .

- **[MLVPN](https://zehome.github.io/MLVPN/)**  
  Multi-link VPN that bonds internet links to increase bandwidth, actively monitoring and removing faulty links without dropping TCP connections [citation:29].

- **[HypoMux](https://github.com/Hypostasis-Cat/HypoMux)**  
  Windows multi-NIC network accelerator combining Ethernet, Wi-Fi, and hotspots for multi-path transmission and smart traffic routing [citation:22].

- **[openppp2](https://github.com/Miaocchi/openppp2)**  
  Layer 2/3 virtual Ethernet overlay engine and programmable VPN/SD-WAN foundation with route steering, split tunneling, and bandwidth aggregation hooks .

- **[YANET2](https://github.com/yanet-platform/yanet2)**  
  High-performance modular software router built on DPDK, functioning as router, firewall, L3 load balancer, and NAT device with kernel-bypass packet processing [citation:30].

### Additional Strong Open-Source Options

- **[Firezone](https://github.com/firezone/firezone)** — Zero-trust remote access and network overlay built on WireGuard.
- **[OpenZiti](https://github.com/openziti/ziti)** — Programmable zero-trust network overlay with embedded SD-WAN-like routing.
- **[NetBox](https://github.com/netbox-community/netbox)** — Source of truth for network automation, often paired with SD-WAN orchestration.
- **[Batfish](https://github.com/batfish/batfish)** — Network configuration analysis to validate routing policies before deployment.
- **OpenWrt-based bonding solutions** — Community firmware (mwan3, MWAN) for multi-WAN failover and load balancing on consumer routers.

**Frameworks for building custom systems**: Combine **OpenMPTCProuter** or **vtrunkd** for link aggregation at the edge, **PolyWAN** for Linux-based multi-WAN failover, **NovaEdge** for Kubernetes-native SD-WAN, and **Prometheus + Grafana** for observability.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Network routing and aggregation tools must comply with local telecommunications regulations and ISP terms of service.
- Self-hosted open-source solutions require proper security hardening and understanding of routing protocols.

---

**Made for network engineers, homelab enthusiasts, SMBs, and developers building resilient, vendor-neutral connectivity.**  
Let's make network routing and traffic aggregation more open, affordable, and efficient.
