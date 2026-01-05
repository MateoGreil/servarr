# Docker Media Server

A Docker Compose configuration for a self-hosted media server with:
- **Jellyfin**: Media streaming and management
- **\*arr tools**: Automated media management (Radarr, Sonarr, etc.)
- **Gluetun**: VPN container for secure torrenting

## Features
- Secure torrenting with Gluetun (WireGuard/AirVPN)
- Automated media organization with \*arr tools
- Lightweight and easy to deploy

## Setup
1. Clone this repo:
   ```bash
   git clone https://github.com/mateogreil/servarr.git
   ```
2. Create an `.env` file with your VPN credentials.
3. Run:
   ```bash
   docker compose up -d
   ```

## Requirements
- Docker and Docker Compose
- WireGuard credentials (for Gluetun)

## Notes
- Configure \*arr tools and qBittorrent via their WebUIs after startup.
- Ignore all generated files (e.g., configs, downloads) via `.gitignore`.
