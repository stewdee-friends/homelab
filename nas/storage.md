# NAS Storage

```text
/srv/nas/
├── Public/
├── Documents/
├── Media/
└── Backup/
```

Permissions:
```text
owner = fatimazahra
group = nasusers
mode  = 2775
```

The current NAS uses the same internal SSD that hosts Ubuntu and services. A same-disk backup helps with accidental deletion but does not protect against SSD failure, laptop failure, theft, or physical damage. Future backup target: independent external storage or another system.
