# Enterprise Network Lab - Cisco Packet Tracer

## Overview

This project represents an enterprise network simulation created in Cisco Packet Tracer.

The goal of this lab was to design and configure a secure and redundant network infrastructure using Cisco technologies.

## Network Features

Implemented technologies:

- VLAN segmentation
- Router-on-a-stick inter-VLAN routing
- HSRP gateway redundancy
- EtherChannel with LACP
- Spanning Tree Protocol
- Port Security
- DHCP Relay
- NAT/PAT Internet access
- ACL-based network security
- Guest Wireless Network

## VLAN Design

| VLAN | Name | Purpose |
|------|------|---------|
| 10 | OFFICE | Employee devices |
| 20 | ADMIN | Administration devices |
| 30 | GUEST | Guest WiFi network |
| 40 | SERVER | Server infrastructure |

## High Availability

HSRP was configured between two routers:

- R1: Active router (higher priority)
- R2: Standby router

Virtual gateway addresses:

| VLAN | Virtual IP |
|------|------------|
| 10 | 192.168.10.1 |
| 20 | 192.168.20.1 |
| 30 | 192.168.30.1 |
| 40 | 192.168.40.1 |

## Security Implementation

Security controls:

- Port Security using sticky MAC addresses
- Guest VLAN isolation
- ACL restrictions between VLANs
- WAN firewall ACL

Examples:

- Guest users cannot access internal VLANs
- Office users have restricted access to Admin network
- Internet access provided through NAT/PAT

## Wireless Network

Guest wireless network:

- SSID: GUEST-WIFI
- Security: WPA2-PSK
- VLAN: 30

The Access Point is connected to SW1 and placed in the Guest VLAN.

## Testing

Verified:

- VLAN connectivity
- HSRP operation
- EtherChannel status
- NAT/PAT translation
- ACL filtering
- Internet connectivity

## Files

- `Enterprise-Network-Lab.pkt` - Cisco Packet Tracer project
- `Topology.png` - Network topology diagram
- `CLI.txt` - Device configurations and verification commands
