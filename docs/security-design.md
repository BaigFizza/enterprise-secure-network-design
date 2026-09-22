# Enterprise Network Security Design

## Overview

The network architecture uses multiple layers of security rather than relying on a single control. The design combines perimeter protection, network segmentation, secure wireless access, authentication, and traffic monitoring to reduce exposure and limit unauthorized access.

## Next-Generation Firewall

A next-generation firewall is positioned between the edge routers and the internal network.

Its responsibilities include:

- Stateful traffic inspection
- Intrusion prevention (IPS)
- Content and application filtering
- VPN connectivity
- Threat protection
- Enforcement of inbound and outbound security policies

Placing the firewall at the network perimeter creates a controlled boundary between external networks and internal enterprise resources.

## Network Segmentation

The internal network is segmented using VLANs so different types of devices and services do not share one unrestricted network.

Example segmentation includes:

| VLAN | Purpose |
|---|---|
| VLAN 10 | Employee / Staff Data |
| VLAN 20 | Voice / IP Phones |
| VLAN 30 | Corporate Wireless |
| VLAN 40 | Servers |
| VLAN 50 | Network Management |

Segmentation reduces unnecessary traffic between systems and allows security policies to be applied based on business function.

## Secure Wireless Access

Corporate wireless access uses **WPA3-Enterprise** with **802.1X authentication**.

This provides stronger authentication than a shared Wi-Fi password and allows individual users or devices to authenticate before receiving network access.

## Access Control

Access between network segments should follow the principle of least privilege.

For example:

- Employee devices should only access services required for business operations.
- User networks should not have unrestricted access to management systems.
- Administrative interfaces should be limited to authorized IT personnel.
- Server access should be restricted according to application requirements.

## Monitoring and Threat Detection

Firewall and network-device logs can be collected for security monitoring.

Relevant events include:

- Repeated authentication failures
- Unusual connection attempts
- Blocked firewall traffic
- Unauthorized access attempts
- Unexpected communication between network segments

Centralized monitoring can help administrators identify suspicious activity and investigate potential security incidents.

## Security Objective

The overall objective is to create a layered enterprise network in which perimeter defenses, segmentation, authentication, access control, and monitoring work together.

This defense-in-depth approach reduces the likelihood that a single compromised device or security control would expose the entire enterprise network.
