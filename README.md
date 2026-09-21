# Homelab Portfolio

Personal infrastructure and self-hosted services lab running on a single Ubuntu Server host.  
Built and maintained as a hands-on learning environment focused on **Docker**, Linux systems administration, networking, and reliable service delivery.

This repository documents the high-level design, technology choices, and operational practices of my home lab. All sensitive information (IPs, credentials, internal hostnames, etc.) has been removed or replaced with placeholders.

---

## Overview

| Category              | Details |
|-----------------------|---------|
| **Host**              | Single Ubuntu Server |
| **Container Runtime** | Docker + Docker Compose |
| **Management**        | Portainer |
| **Storage**           | Network-attached storage (NAS) in JBOD configuration |
| **Remote Access**     | WireGuard VPN (wg-easy) + Dynamic DNS (FreeDNS) |
| **Primary Focus**     | Docker-based service deployment, media services, home automation, and infrastructure management |

The lab runs a mix of containerized workloads and native Linux services. The majority of application services are deployed as Docker containers and managed through Portainer. Media and bulk data are stored on a dedicated NAS using JBOD.

---

## Key Technology Stack

**Core Infrastructure**
- Ubuntu Server
- Docker & Docker Compose
- Portainer
- WireGuard (wg-easy)
- AdGuard Home
- Syncthing

**Media Services**
- Jellyfin (media server)
- Immich (photo management)
- Audiobookshelf
- Booklore
- RomM
- Supporting automation and request tools

**Home Automation**
- Home Assistant
- Zigbee2MQTT
- MQTT (Mosquitto)
- SLZB-06M Zigbee coordinator

**AI / Local LLM**
- Ollama
- Open WebUI

**Supporting Services**
- NTFY
- Notifiarr
- Watchtower
- Homepage / Glance dashboards
- Crafty Controller
- Termix
- QDirStat
- QNAP NAS integration

---

## Design Principles

- Prefer Docker containers for application workloads
- Centralized management via Portainer
- Secure remote access via WireGuard VPN (no direct exposure of services)
- Dynamic DNS for reliable remote connectivity
- Media storage on a dedicated NAS using JBOD for flexible capacity expansion
- Clear separation of concerns across service categories
- Infrastructure changes tracked and documented

---

## Repository Contents

- [`docs/architecture.md`](docs/architecture.md) – High-level design and component overview
- [`docs/media-services.md`](docs/media-services.md) – Media servers and related tools
- [`docs/networking-access.md`](docs/networking-access.md) – VPN, DNS, and remote access
- [`docs/home-automation.md`](docs/home-automation.md) – Home Assistant and Zigbee
- [`docs/management-tools.md`](docs/management-tools.md) – Portainer, monitoring, and utilities
- [`docs/lessons-learned.md`](docs/lessons-learned.md) – Practical takeaways and improvements
- [`examples/`](examples/) – Sanitized configuration patterns

---

## Skills Demonstrated

- Docker containerization and multi-container application management
- Linux systems administration (Ubuntu Server)
- Secure remote access design (WireGuard + Dynamic DNS)
- Service orchestration and dependency management
- Integration of Docker workloads with network-attached storage (NAS / JBOD)
- Self-hosted media platform deployment
- Home automation integration
- Documentation and infrastructure organization
- Troubleshooting and iterative improvement of self-hosted services

---

## Notes

This is a personal learning and experimentation environment. It is **not** a production system.  
Configurations shown in this repository are sanitized examples only.

---

## Contact

Feel free to open an issue if you have questions about the design decisions or tooling choices documented here.
