# Enterprise Network Lab - Cisco Packet Tracer

![Network Topology](Topology.png)

## Overview

This project simulates an enterprise office network designed and configured in Cisco Packet Tracer.

The network includes multiple departments separated using VLANs, redundant gateway configuration, Layer 2 security, wireless guest access and Internet connectivity.

## Implemented Technologies

- VLAN segmentation
- Router-on-a-Stick inter-VLAN routing
- HSRP gateway redundancy
- EtherChannel with LACP
- Spanning Tree Protocol (PVST)
- Port Security
- DHCP Relay
- NAT/PAT overload
- ACL-based traffic filtering
- WAN firewall rules
- Guest Wireless Network

## VLAN Design

| VLAN | Name | Purpose |
|------|------|---------|
| 10 | OFFICE | Employee users |
| 20 | ADMIN | Administration users |
| 30 | GUEST | Guest WiFi users |
| 40 | SERVER | Internal servers |

## Network Security

Implemented security policies:

- Guest VLAN isolated from internal VLANs
- Office users restricted from Admin network
- Server access controlled using ACL rules
- Port Security enabled on access ports
- WAN traffic filtered using extended ACL

## High Availability

HSRP configured between R1 and R2:

- Virtual gateway: 192.168.x.1
- R1 configured as Active router
- R2 configured as Standby router

## Verification

CLI verification outputs are available in:

`CLI.txt`

Packet Tracer simulation file:

`RedundancyNetwork.pkt`
