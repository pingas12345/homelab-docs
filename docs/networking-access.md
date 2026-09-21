# Networking & Remote Access

## Remote Access Design

Secure remote access to the home network is provided by a WireGuard VPN.

- **VPN Solution**: wg-easy (WireGuard)
- **Dynamic DNS**: FreeDNS
- **Access Method**: Clients connect via WireGuard; no individual services are directly exposed to the public internet except for VPN setup and game servers.

This approach provides encrypted access to the entire home network while minimizing the external attack surface.

## DNS & Filtering

- **AdGuard Home** is used for network-wide DNS resolution and filtering.

## Key Principles

- Prefer VPN access over port forwarding individual services
- Keep management interfaces (Portainer, etc.) internal or VPN-only
- Use dynamic DNS to handle changing public IP addresses
- Maintain clear separation between externally reachable endpoints and internal services

## Skills Demonstrated

- Secure remote access design
- WireGuard VPN deployment and management
- Dynamic DNS configuration
- Network-level DNS filtering
- Reducing external exposure of services
