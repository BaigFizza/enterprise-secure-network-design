# Enterprise Secure Network Design

A secure and scalable enterprise network architecture designed for a simulated organization with 678 employees across two buildings.

## Project Overview

This project designs a modern network infrastructure to replace an outdated enterprise network environment. The goal is to support hundreds of users while improving network performance, scalability, reliability, wireless connectivity, and security.

The proposed environment uses a high-speed fiber backbone, departmental network segmentation, secure wireless access, and Quality of Service (QoS) policies to support different types of business traffic.

## Project Goals

- Design a scalable network for 678 employees across two buildings
- Segment departments to improve network security and traffic management
- Estimate network traffic and bandwidth requirements
- Design a 10 Gbps backbone for high-capacity communication
- Provide secure enterprise wireless connectivity
- Prioritize latency-sensitive applications using QoS
- Improve network reliability and scalability

## Network Design Highlights

- 10 Gigabit Ethernet backbone
- Fiber connectivity between buildings
- Layer 3 switching
- Department-based VLAN segmentation
- Wi-Fi 6 wireless infrastructure
- WPA3-Enterprise wireless security
- 802.1X authentication
- Separate employee and guest wireless networks
- Next-generation firewall and IDS/IPS
- Quality of Service (QoS) for VoIP, video, and business applications

## Traffic & Capacity Planning

The network was designed around estimated traffic requirements for different departments and services.

Estimated internal traffic is approximately **2.9 Gbps**, with additional demand from wireless devices and communication between buildings.

Peak wireless usage is estimated at approximately **0.8–1.2 Gbps**, while inter-building traffic may reach approximately **1–1.5 Gbps**.

Based on these requirements, a **10 Gbps fiber backbone** provides sufficient capacity for current traffic while allowing room for future growth.

## Quality of Service (QoS)

QoS policies prioritize applications based on their sensitivity to latency, jitter, and packet loss.

| Traffic Type | QoS Target |
|---|---|
| VoIP | < 150 ms latency |
| Video | < 200 ms latency |
| Jitter | < 30 ms |
| VoIP Packet Loss | < 1% |
| Critical Data | Near-zero packet loss |

Traffic prioritization includes:

- **EF** — VoIP
- **AF41/42** — Video
- **AF21/22** — Business applications

## Security Approach

The network design uses multiple layers of security, including:

- Department-based VLAN segmentation
- WPA3-Enterprise
- 802.1X authentication
- Next-generation firewall protection
- IDS/IPS monitoring
- Isolated guest wireless access
- Network access controls

## Project Status

This repository documents the design and analysis of the network architecture. Additional diagrams, traffic analysis, security documentation, and design details will be added as the project is developed.
