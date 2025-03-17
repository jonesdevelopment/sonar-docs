---
description: >-
  Sonar includes a feature that allows players to be automatically transferred
  back to the origin server after successfully passing bot verification,
  introduced in Minecraft version 1.20.5.
---

# Using 1.20.5+ transfers

Set to true to enable the transfer feature. **Ensure the feature is enabled in your server's configuration** and **consider adjusting login rate-limiting settings in Velocity or other proxies/plugins to avoid transfer issues**. Default is false.

* Set the login ratelimit in Velocity to 1000 (or disable it)—the BungeeCord and Bukkit equivalent is connection throttling.
* Enable transfers in velocity.toml (Velocity); config.yml (BungeeCord); server.properties (Bukkit)

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

{% hint style="info" %}
If your server allows Bedrock players to join via Geyser, make sure to set up [TransferTool](https://github.com/onebeastchris/TransferTool) for Geyser, so Bedrock players are redirected to the correct server.
{% endhint %}
