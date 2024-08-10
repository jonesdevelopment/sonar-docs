---
description: >-
  These settings control general behavior for Sonar, including update checks,
  logging, and player limits.
---

# General settings

Enables automatic update checks using the GitHub API to ensure Sonar is up to date. Default: `true`

```yaml
check-for-updates: true
```

Determines whether Sonar logs players' IP addresses in the console. Default: `true`

```yaml
log-player-addresses: true
```

The number of players allowed to be online with the same IP address. If you have a server where people are allowed to use many alt accounts, you might want to increase this number. Any player who tries joining when there are already more than the maximum number of players using the same IP address online will be kicked. Default: `3`

```yaml
max-online-per-ip: 3
```
