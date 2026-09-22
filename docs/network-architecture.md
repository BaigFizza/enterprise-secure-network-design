# Enterprise Network Architecture

## Architecture Overview

This project uses a hierarchical enterprise network design to support a simulated organization with 678 employees across two buildings.

The architecture separates the network into edge, core, distribution, and access functions. This structure improves scalability, simplifies network management, and allows security and performance policies to be applied at appropriate points in the network.

## Internet Edge

Two edge routers provide connectivity between the enterprise network and external service providers.

Using redundant edge connectivity reduces dependence on a single network path and provides additional resilience if one connection becomes unavailable.

Traffic entering or leaving the internal network passes through the next-generation firewall before reaching enterprise resources.

## Core Layer

The core layer provides high-speed connectivity between major parts of the network.

Two core switches are used to provide redundancy and support high availability.

The core infrastructure uses **10 GbE connectivity** to provide sufficient capacity for current traffic requirements while allowing room for future growth.

## Distribution Layer

Each building contains distribution switching that connects the building's access infrastructure to the core network.

The distribution layer provides a logical point for:

- VLAN routing
- Traffic aggregation
- Access-control policies
- QoS enforcement
- Connectivity between access and core infrastructure

## Access Layer

Access switches provide network connectivity to end-user devices such as:

- Employee workstations
- IP phones
- Wireless access points
- Printers
- Other enterprise endpoints

Devices are separated into VLANs according to their function and security requirements.

## Inter-Building Connectivity

The two buildings are connected through high-speed fiber infrastructure.

The design uses a **10 GbE backbone** to accommodate estimated inter-building traffic while providing additional capacity for traffic growth and peak utilization.

## Wireless Infrastructure

Wi-Fi 6 access points provide wireless connectivity throughout both buildings.

Corporate wireless access uses WPA3-Enterprise and 802.1X authentication.

Guest wireless traffic is logically separated from internal enterprise resources to reduce security exposure.

## High Availability and Scalability

Redundancy is incorporated into critical portions of the architecture, including the edge and core layers.

The network is designed so additional users, access switches, wireless access points, and network segments can be introduced without requiring a complete redesign of the infrastructure.

## Design Summary

The architecture combines hierarchical network design, high-speed backbone connectivity, segmentation, redundancy, secure wireless access, and traffic management.

Together, these components provide a scalable foundation for supporting enterprise users and business applications across multiple buildings.
