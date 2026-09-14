# Security Model

## Authentication
- Linux administration uses the Linux account and sudo.
- Samba uses an authenticated account; guest access is disabled.
- SFTPGo uses `nasuser`; TOTP 2FA is enabled.
- Tailscale provides the private remote path.

## Filesystem
```text
owner = fatimazahra
group = nasusers
mode  = 2775
```
The setgid bit causes new files/directories to inherit the `nasusers` group. The SFTPGo service account is a member of `nasusers`.

## Firewall intent
```text
default deny incoming
default allow outgoing
```
Only required services are allowed from trusted LAN/Tailscale ranges.

## Local vs network access
Opening `/srv/nas` directly on Zahra is Linux filesystem access. A Samba password does not automatically protect direct local filesystem browsing. Local access is controlled by Linux users/groups/permissions; Samba and SFTPGo authentication apply to access through those services.

## Secrets
Never commit passwords, `.env` secrets, TOTP seeds/recovery codes, private keys, API tokens, router credentials, or Tailscale auth keys.
