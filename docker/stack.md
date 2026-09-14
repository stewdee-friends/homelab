# Docker Stack

| Application | Image |
|---|---|
| Homepage | `ghcr.io/gethomepage/homepage:latest` |
| Uptime Kuma | `louislam/uptime-kuma:1` |
| Portainer | `portainer/portainer-ce:latest` |
| Dozzle | `amir20/dozzle:latest` |
| Netdata | `netdata/netdata:stable` |

Expected ports: Homepage 3000, Uptime Kuma 3001, Portainer 9000, Dozzle 8888, Netdata 19999.

Current state: containers were preserved, but expected web ports were not exposing correctly during the latest troubleshooting. Docker recovery is intentionally deferred.

Homepage configuration is under `/opt/homepage/config/` and uses `/var/run/docker.sock`. Do not commit private configuration or secrets.
