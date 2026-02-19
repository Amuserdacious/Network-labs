Lab 5: Small Office Network with DHCP

Date: 2026/02/19

Objective
Simulate a small office network with:
- 3 wired PCs
- 1 printer
- 1 wireless laptop
- All devices get IPs automatically from the router (DHCP)

Devices Used
- Router: Cisco 2911
- Switch: Cisco 2960-24TT
- Wireless Router: WRT300N (acts as access point)
- 3 x PCs, 1 x Printer, 1 x Laptop

Topology
- Router connected to switch (Gi0/0)
- Switch connected to:
  - PC1 (Fa0/1)
  - PC2 (Fa0/2)
  - PC3 (Fa0/3)
  - Printer (Fa0/4)
  - WRT300N (Fa0/5) – for wireless laptop

Configuration Highlights
- Enabled DHCP on the router (pool for 192.168.1.0/24)
- Switch ports in default VLAN 1 (access mode)
- Wireless router set to wireless bridge (disable DHCP)
- Laptop connected via WiFi

Testing
- All devices obtained IP addresses from router
- Verified connectivity:
  - Wired PC ↔ Printer
  - Wired PC ↔ Wireless Laptop
  - All devices can ping the router (default gateway)
