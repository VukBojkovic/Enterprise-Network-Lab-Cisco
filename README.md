# Cisco Enterprise Network Project

## Topology

![Network Topology](Topology.png)

## Project Overview

This project simulates a small enterprise network built in Cisco Packet Tracer.

Implemented technologies:

- VLANs (10, 20, 30, 40)
- Router-on-a-Stick
- HSRP Gateway Redundancy
- EtherChannel (LACP)
- STP
- Port Security
- DHCP Relay
- NAT/PAT
- ACL Security Policies
- Guest WiFi Network

## VLAN Design

| VLAN | Name | Purpose |
|---|---|---|
| 10 | OFFICE | Employee devices |
| 20 | ADMIN | Administration |
| 30 | GUEST | Guest WiFi |
| 40 | SERVER | Server network |

## Security Features

- Port Security on access ports
- Guest VLAN isolation
- ACL filtering between VLANs
- WAN firewall rules
- NAT overload for Internet access

## Verification

Configuration outputs can be found in:

`CLI.txt`

The Packet Tracer file:

`Network_Project.pkt`
