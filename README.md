# AiTECH Manager

**Secure VPS provisioning and multi-protocol networking management for Ubuntu and Debian servers.**

[![Latest Release](https://img.shields.io/github/v/release/Alouk0/aitech-manager-releases?display_name=tag&style=flat-square)](https://github.com/Alouk0/aitech-manager-releases/releases/latest)
[![Platforms](https://img.shields.io/badge/platforms-Ubuntu%2020.04%2B%20%7C%20Debian%2011%2B-2F3A4A?style=flat-square&logo=linux&logoColor=white)](#supported-platform)
[![Architecture](https://img.shields.io/badge/architecture-amd64-2F3A4A?style=flat-square)](#supported-platform)
[![License](https://img.shields.io/badge/license-proprietary-1F6FEB?style=flat-square)](#licensing)

> This repository is the official checksum-verified binary distribution channel for AiTECH Manager.

## Overview

AiTECH Manager is a licensed infrastructure platform that automates fresh-VPS provisioning, encrypted networking services, client lifecycle management, security enforcement, and production service operations from one consistent interface.

### Managed Services

- OpenSSH, Dropbear, Stunnel and SSH WebSocket
- OpenVPN UDP, TCP and RFC 6455/WSS
- Xray WebSocket, XHTTP and gRPC transports
- Hysteria2, DNSTT and BadVPN UDPGW
- Nginx, TLS certificates, firewall and systemd lifecycle

### Operational Capabilities

- Automated domain and DNS validation
- TLS certificate provisioning and verification
- Client creation, deletion, renewal and credential management
- Expiry, bandwidth quota and connection-limit enforcement
- Online-session observation and service diagnostics
- Atomic configuration writes and rollback-safe deployment
- Checksum-pinned, deterministic production releases

## Current Release

**[AiTECH Manager 1.2.0 WebSocket Pro](https://github.com/Alouk0/aitech-manager-releases/releases/tag/v1.2.0-websocket-pro.1)**

WebSocket Pro adds a dedicated OpenVPN RFC 6455/WSS bridge, persistent systemd lifecycle, HTTPS-only Nginx routing, Manager status integration, provisioning integration, backend recovery and reboot persistence.

## Supported Platform

- Ubuntu 20.04 LTS, 22.04 LTS, and 24.04 LTS
- Debian 11, 12, and 13
- Linux amd64
- Root or passwordless sudo access
- A public domain with its DNS A record pointing to the VPS
- Public TCP ports 80 and 443 available for certificate and HTTPS services

## Licence Access

AiTECH Manager requires a valid licence key. For licensing, pricing, installer access, or deployment support, contact AiTECH NETWORKS directly:

[![Message on Telegram](https://img.shields.io/badge/Message_on_Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/Aluk0)

## Installation

Run on a clean supported VPS:

```bash
curl -fsSL --proto "=https" --tlsv1.2 https://install.fastlysmarty.co.uk/install.sh -o /tmp/aitech-install.sh && sudo bash /tmp/aitech-install.sh
```

The installer downloads immutable GitHub release assets, verifies their pinned SHA-256 checksums, validates the licence public key, and stops safely if any integrity check fails.

## OpenVPN WebSocket Compatibility

The server publishes OpenVPN TCP through RFC 6455/WSS at `/openvpnws`. Stock OpenVPN clients do not provide native WebSocket transport, so clients must use a compatible WebSocket-capable application or companion tunnel.

## Security

Do not report vulnerabilities through public issues. Use GitHub private vulnerability reporting through the repository **Security** tab.

Release binaries, installers and offline archives are published with SHA-256 checksum files.

## Support

- [Latest release](https://github.com/Alouk0/aitech-manager-releases/releases/latest)
- [Release history](https://github.com/Alouk0/aitech-manager-releases/releases)
- [Issue tracker](https://github.com/Alouk0/aitech-manager-releases/issues)

## Licensing

AiTECH Manager is proprietary software. Access and use require a valid AiTECH Manager licence. Distribution assets in this repository do not grant permission to copy, modify, reverse engineer or redistribute the software outside the applicable licence terms.

---

<div align="center"><sub>Powered by AiTECHNETWORKS LIMITED RC 1900411</sub></div>
