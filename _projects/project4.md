---
layout: project
title: "Laptop DHCP and PXE Server"
description: "Transform your laptop into a DHCP and PXE server using Docker Compose. Automatically assign IP addresses and enable network booting via PXE with flexible network configurations leveraging built-in Wi-Fi and wired interfaces."
permalink: /notepc/
github_url: "https://github.com/superdoccimo/notepc"
---

This project provides Docker Compose files and detailed setup instructions to configure a laptop as a DHCP and PXE server. By leveraging both Wi-Fi and wired network interfaces, it allows client devices within your network to automatically receive IP addresses and boot over the network via PXE.

**Key Features:**

- **Automated IP Assignment:** Set up a DHCP server using Docker Compose to automatically assign IP addresses.
- **PXE Boot Capability:** Enable network booting for client devices through PXE.
- **Flexible Network Configuration:** Utilize Netplan on Ubuntu for customizable network setups, accommodating both static and DHCP configurations.
- **Custom Docker Network:** Create a fixed custom Docker network to ensure a consistent IP range.
- **NAT and IP Forwarding:** Configure IP forwarding and NAT to route traffic effectively.

Clone the repository, adjust your network interface settings as needed, and deploy the Docker Compose setup to transform your laptop into a fully functional DHCP and PXE server.
