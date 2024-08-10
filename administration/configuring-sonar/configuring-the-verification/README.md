---
description: >-
  Sonar uses a lightweight limbo server to perform advanced bot checks on new
  players joining for the first time. These settings control when and how these
  bot verifications are conducted.
---

# Configuring the verification

Determines when new players are verified. Options:

* `ALWAYS`: All new players are checked (Recommended)
* `DURING_ATTACK`: Players are only checked during an attack
* `NEVER`: No verification for new players

Default: `ALWAYS`

```yaml
timing: ALWAYS
```

Sets the gamemode during verification. Options:&#x20;

* `SURVIVAL`: all UI components are visible
* `CREATIVE`: all UI components are hidden
* `ADVENTURE`: all UI components are visible (Recommended)

Default: `ADVENTURE`

```yaml
gamemode: ADVENTURE
```

Specifies the username used in the cached LoginSuccess packet. Default: `Sonar`

```yaml
cached-username: Sonar
```

Logs all new verification attempts. Default: `true`

```yaml
log-connections: true
```

Logs verification attempts only during attacks. Default: `false`

```yaml
log-during-attack: false
```

Logs all player movements during verification, useful for debugging. Not recommended for production servers. Default: `false`

```yaml
debug-xyz-positions: false
```

Enables verification checks for Geyser (Bedrock) players. This is experimental and may cause issues. Default: `true`

```yaml
check-geyser-players: true
```

The time (in milliseconds) before disconnecting a player if they stop sending packets. Default: `8000`

```yaml
read-timeout: 8000
```

The time (in milliseconds) before disconnecting a player if the server stops sending packets. Default: `10000`

```yaml
write-timeout: 10000
```

The cooldown period (in milliseconds) before a player can reconnect during verification. Default: `8000`

```yaml
rejoin-delay: 8000
```

The duration (in milliseconds) for which Sonar remembers the number of failed verifications for a player. Default: `120000`

```yaml
remember-time: 120000
```

The duration (in milliseconds) an IP is blocked after repeated verification failures. Default: `600000`

```yaml
blacklist-time: 600000
```

The number of failed verifications before an IP is blacklisted. Set to `0` to disable blacklisting. Default: `2`

```yaml
blacklist-threshold: 2
```

A list of protocol IDs that are blocked from joining the server. Default: `[]` (empty)

```yaml
blacklisted-protocols: []
```
