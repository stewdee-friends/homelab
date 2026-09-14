# Access Matrix

Replace placeholders locally if needed. Do not commit real secrets.

| Service | LAN | Tailscale | Authentication |
|---|---|---|---|
| SMB Public | `\\<ZAHRA_LAN_IP>\Public` | `\\<ZAHRA_TAILSCALE_IP>\Public` | Samba account |
| SMB Documents | `\\<ZAHRA_LAN_IP>\Documents` | `\\<ZAHRA_TAILSCALE_IP>\Documents` | Samba account |
| SMB Media | `\\<ZAHRA_LAN_IP>\Media` | `\\<ZAHRA_TAILSCALE_IP>\Media` | Samba account |
| SMB Backup | `\\<ZAHRA_LAN_IP>\Backup` | `\\<ZAHRA_TAILSCALE_IP>\Backup` | Samba account |
| Cockpit | `https://<ZAHRA_LAN_IP>:9090` | `https://<ZAHRA_TAILSCALE_IP>:9090` | Linux user |
| SFTPGo WebAdmin | `http://<ZAHRA_LAN_IP>:8080/web/admin` | `http://<ZAHRA_TAILSCALE_IP>:8080/web/admin` | SFTPGo admin |
| SFTPGo WebClient | `http://<ZAHRA_LAN_IP>:8080/web/client` | `http://<ZAHRA_TAILSCALE_IP>:8080/web/client` | `nasuser` + TOTP |
| SSH | `<ZAHRA_LAN_IP>:22` | `<ZAHRA_TAILSCALE_IP>:22` | Linux user |
