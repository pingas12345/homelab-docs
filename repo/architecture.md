# Architecture Overview

## Host Environment

- **Operating System**: Ubuntu Server
- **Container Runtime**: Docker + Docker Compose
- **Container Management**: Portainer
- **Primary Goal**: Reliable, maintainable self-hosted services with a strong focus on containerization

The lab runs on a single physical host. Application workloads are primarily delivered as Docker containers, while core system services remain native where appropriate.

## High-Level Design
