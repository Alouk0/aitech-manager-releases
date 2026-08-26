# Changelog

All notable public AiTECH Manager releases and distribution-channel revisions are documented here.

## [v1.2.0-websocket-pro.1] — 2026-08-26

### Installer and Distribution

- Added professional Telegram guidance for licence access and deployment support.
- Added explicit Ubuntu and Debian platform documentation.
- Added private vulnerability-reporting guidance and security policy.
- Added structured customer-facing release notes.
- Rebuilt and checksum-verified the deterministic offline bundle.

### Binary

- No production binary changes.
- Binary SHA-256 remains `bc6efa7b632872a86c429dd70eab47638dd8cf62616c4547a0356758e824d727`.

## [v1.2.0-websocket-pro] — 2026-08-26

### Added

- OpenVPN TCP transport over RFC 6455 WebSocket/WSS.
- Public TLS `/openvpnws` endpoint through Nginx.
- Loopback-only OpenVPN WebSocket bridge on `127.0.0.1:8882`.
- Dedicated systemd service with restart recovery and boot persistence.
- OpenVPN Manager WebSocket service information.
- Automatic WebSocket service provisioning during installation.

### Validated

- Fresh-VPS installation and post-reboot persistence.
- RFC 6455 handshake, framing, fragmentation, ping/pong and close handling.
- Concurrent public WSS sessions and binary data fidelity.
- Backend failure and recovery without bridge restart.
- Existing OpenVPN UDP, OpenVPN TCP and SSH WebSocket compatibility.
- Deterministic Go build and complete Go test suite.

### Security

- Loopback-only bridge listener.
- TLS termination at the managed Nginx edge.
- Backend reachability validation and controlled HTTP rejection responses.
- Checksum-pinned public installer and release assets.

## [v1.2.0-r2]

Previous production release before the WebSocket Pro transport integration.

[v1.2.0-websocket-pro.1]: https://github.com/Alouk0/aitech-manager-releases/releases/tag/v1.2.0-websocket-pro.1
[v1.2.0-websocket-pro]: https://github.com/Alouk0/aitech-manager-releases/releases/tag/v1.2.0-websocket-pro
[v1.2.0-r2]: https://github.com/Alouk0/aitech-manager-releases/releases/tag/v1.2.0-r2

Powered by AiTECHNETWORKS LIMITED RC 1900411
