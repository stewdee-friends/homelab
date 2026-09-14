# Current State

## Server
- Hostname: `Zahra`
- OS: Ubuntu Desktop 24.04.5 LTS
- CPU: 2 cores
- RAM: approximately 4 GB
- Storage: approximately 128 GB internal SSD
- Primary Linux user: `fatimazahra`

## Network
Private values are intentionally sanitized.
- LAN subnet: `<HOME_LAN_SUBNET>`
- Zahra LAN IP: `<ZAHRA_LAN_IP>`
- Zahra Tailscale IP: `<ZAHRA_TAILSCALE_IP>`
- Router: `<HOME_ROUTER>`
- Windows client: `<WINDOWS_CLIENT_IP>`

## Completed
- NAS directories and Samba shares
- Windows SMB read/write verification
- `nasusers` group and setgid permissions
- Tailscale private remote access
- Cockpit LAN/Tailscale access
- SFTPGo LAN/Tailscale WebClient access
- SFTPGo `nasuser` with `/srv/nas` root
- TOTP 2FA for `nasuser`
- UFW restricted-source rules

## Known limitation
Docker containers exist, but expected web ports were not exposing correctly during the latest troubleshooting. Docker recovery is intentionally deferred.

## Next
Backup design and implementation.
