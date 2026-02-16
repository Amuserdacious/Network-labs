Date: 2026/02/16

What I Did
- Created VLAN 10 (SALES) and VLAN 20 (IT)
- Assigned ports:
  - Gi1/0/1 and Gi1/0/3 → VLAN 10
  - Gi1/0/2 → VLAN 20
  Set IPs:
  - PC1: 192.168.10.10 (VLAN 10)
  - PC2: 192.168.20.20 (VLAN 20)
  - PC3: 192.168.10.30 (VLAN 10)

Results:
 PC1 can ping PC3 (same VLAN)
 PC1 cannot ping PC2 (different VLANs)

Why
VLANs isolate traffic. Different VLANs = different networks.
