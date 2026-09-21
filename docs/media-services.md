# Media Services

Self-hosted media platform providing video, photo, audiobook, ebook, and related content services. All components run as Docker containers and are managed through Portainer.

Media files are stored on a dedicated NAS configured in JBOD (Just a Bunch Of Disks), providing flexible capacity expansion.

## Core Components

- **Jellyfin** - Media server for video and music
- **Immich** - High-performance photo and video backup & management
- **Audiobookshelf** - Audiobook and podcast server
- **Booklore** - Ebook library management
- **RomM** - ROM library management

## Supporting Tools

Additional containers provide automation, request handling, notifications, and library maintenance. These tools integrate with the core media services to improve usability and reduce manual work.

## Storage

- Media libraries reside on a network-attached storage (NAS) device
- NAS is configured in JBOD mode for straightforward capacity scaling
- Docker containers access media via network mounts / bind mounts

## Operational Notes

- Services are deployed using Docker Compose patterns
- Persistent application data is stored on dedicated volumes
- Access is restricted to the local network and WireGuard VPN
- Regular updates are handled via Portainer and Watchtower (where appropriate)

## Skills Demonstrated

- Multi-container application deployment
- Service dependency management
- Integration of Docker workloads with network-attached storage
- Persistent storage configuration across host and NAS
- Operational maintenance of a media platform
