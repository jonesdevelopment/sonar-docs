---
description: >-
  The attack tracker in Sonar monitors for potential bot attacks based on player
  activity. Adjust these settings only if you are familiar with the system's
  operation.
---

# Adjusting the attack tracker

The minimum number of new players required to trigger attack detection. Default: `8`

```yaml
min-players-for-attack: 8
```

The minimum duration (in milliseconds) that an attack must last to be considered ongoing. Default: `30000`

```yaml
min-attack-duration: 30000
```

The minimum number of incident reports needed to confirm an attack, acting as a buffer against false positives. Default: `2`

```yaml
min-attack-threshold: 2
```

The cooldown period (in milliseconds) required before detecting a new attack after one has ended. Default: `3000`

```yaml
attack-cooldown-delay: 3000
```
