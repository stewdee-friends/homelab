# Zahra Homelab Topology

```text
                    HOME NETWORK
                 <HOME_LAN_SUBNET>
                         |
                   Home Router
                         |
                  +------v------+
                  |    Zahra    |
                  | Ubuntu 24.04|
                  +------+------+ 
                         |
          +--------------+---------------+
          |              |               |
        /srv/nas       Services        Docker
          |              |               |
     +----+----+     Cockpit          Homepage
     |    |    |     SFTPGo            Uptime Kuma
 Public Docs Media                     Portainer
     |                               Dozzle
   Backup                            Netdata

Tailscale
   |
   +---- encrypted private path ----> Zahra
```

The design intentionally keeps NAS services private and uses Tailscale instead of public port forwarding.
