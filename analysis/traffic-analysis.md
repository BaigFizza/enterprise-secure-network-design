# Network Traffic & Capacity Analysis

## Overview

This analysis estimates network traffic requirements for a simulated 678-user enterprise environment across two buildings. The goal is to determine whether the proposed network infrastructure provides sufficient capacity for normal business operations while allowing room for peak utilization and future growth.

## Estimated Traffic Demand

The network must support several categories of traffic, including:

- General employee data traffic
- Web and cloud application usage
- Voice and collaboration traffic
- Wireless devices
- File transfers and internal services
- Communication between buildings

Based on the estimated usage patterns, internal network traffic is approximately **2.9 Gbps**, while wireless demand is estimated at approximately **0.8–1.2 Gbps**.

Inter-building traffic is expected to range from approximately **1–1.5 Gbps** depending on workload and peak utilization.

## Capacity Planning

To prevent the network backbone from becoming a bottleneck, the proposed architecture uses **10 GbE backbone connections** between the core and distribution layers.

This provides additional capacity beyond the estimated normal traffic demand and allows the network to accommodate:

- Peak traffic periods
- Increased wireless usage
- Large internal file transfers
- Additional users and devices
- Future network expansion

## Design Decision

A 10 GbE backbone was selected because the estimated enterprise traffic remains well below the available backbone capacity during normal operation.

This capacity margin helps maintain network performance while providing room for traffic spikes and organizational growth.
