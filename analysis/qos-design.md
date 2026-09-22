# Quality of Service (QoS) Design

## Overview

Quality of Service (QoS) is used to prioritize important network traffic when multiple applications compete for available bandwidth.

For this enterprise network, traffic is divided into different priority levels based on how sensitive each service is to delay, latency, and packet loss.

## Traffic Prioritization

| Traffic Type | Priority | QoS Treatment |
|---|---|---|
| Voice / VoIP | Critical | Highest priority |
| Video Conferencing | High | Prioritized |
| Business Applications | High | Prioritized |
| General Web Traffic | Normal | Best effort |
| Email | Normal | Best effort |
| Large File Transfers | Low | Lower priority during congestion |
| Guest Wireless Traffic | Low | Limited priority |

## QoS Strategy

### Voice and Real-Time Traffic

Voice and other real-time communication services receive the highest priority because latency, jitter, and packet loss can noticeably affect call quality.

### Business-Critical Applications

Applications required for normal business operations receive priority over general web browsing and non-critical traffic.

### General User Traffic

Standard web browsing and email traffic use normal best-effort delivery because small delays generally do not significantly affect usability.

### Bulk Traffic

Large downloads, backups, and other bandwidth-intensive transfers receive lower priority during periods of congestion so they do not interfere with time-sensitive services.

## Design Goal

The purpose of this QoS strategy is not to increase total bandwidth. Instead, it ensures that available bandwidth is allocated intelligently when the network becomes congested.

Combined with the proposed 10 GbE backbone, this approach helps maintain reliable performance for critical enterprise applications while still supporting normal user traffic.
