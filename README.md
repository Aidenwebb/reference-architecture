# Reference Architecture
Reference network architecture built using GitDevSecOps

## Overview

### 1.0.32.0/19 - Our fictional Internet IPv4 address space
Chosen as the IP range falls within China's public internet subnet space, so it is unlikely to conflict with many online resources we may want to access should this lab ever need connections to the real-world internet

### NexaNet - Our fictional ISP

Exists only to provide a quasi-realistic interconnect between different lab site networks

- Domain: Nexanet.fake
- WAN Address space: 1.0.32.0/19
- LAN Address space: 172.16.0.0/24

### Greg Andrews

Represents a typical internet user on their home network.

- WAN address space: 1.0.33.0/24
  - Gateway: 1.0.33.1
  - Public IP: 1.0.33.2
- LAN address space: 192.168.100/24

### MagpieLabs

Represents our model business for this architecture lab.

- Domain: magpielabs.win
- WAN Address space: 1.0.34.0/28
  - Gateway: 1.0.34.1/28
  - Public IPs: 1.0.34.2/28 - 1.0.34.14/28
- LAN Address space: 10.0.0.0/24
