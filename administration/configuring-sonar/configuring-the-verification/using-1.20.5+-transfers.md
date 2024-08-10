---
description: >-
  Sonar includes a feature that allows players to be automatically transferred
  back to the origin server after successfully passing bot verification,
  introduced in Minecraft version 1.20.5.
---

# Using 1.20.5+ transfers

Set to true to enable the transfer feature. Ensure the feature is enabled in your server's configuration and consider adjusting login rate-limiting settings in Velocity or other proxies/plugins to avoid transfer issues. Default is false.

```yaml
enabled: false
```

Specify the server IP or domain where players should be transferred after verification. This is the IP or domain used by players to connect to your server (e.g., play.my-server.com).

```yaml
destination-host: play.my-server.com
```

Define the port for the origin server connection. The default is 25565, which is standard unless your server requires a different port.

```yaml
destination-port: 25565
```

For a detailed setup guide, refer to the [YouTube tutorial](https://youtu.be/aSWrzQVjGnc?t=71).
