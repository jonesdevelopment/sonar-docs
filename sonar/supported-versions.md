---
description: List of all supported Minecraft versions and server software
---

# Supported versions

**Supported client versions**

* **Minecraft: Java Edition** 1.7.2-1.21.3
* **Minecraft: Bedrock Edition** is handled through [GeyserMC](https://geysermc.org/)

**Software requirements**

* [Velocity](https://papermc.io/downloads/velocity) (3.3.0 build 330 or above)
* [BungeeCord](https://ci.md-5.net/job/BungeeCord/) (1.20 or above)
* [Paper](https://papermc.io/downloads/paper) (1.8.8 or above)
  * **Bukkit and Spigot are supported**, but it is recommended to use Paper or another server fork.

**Dependency requirements**

* [Netty](https://netty.io/) 4.1 (or above)
  * If your server depends on an older Netty version (1.7.2-1.8.8 servers mainly have this problem), please consider using an updated fork such as [PandaSpigot](https://github.com/hpfxd/PandaSpigot) (or similar alternatives).

{% hint style="warning" %}
**Disclaimer**

* It's possible that some highly altered server forks won't be supported.
* Some significantly modified Minecraft clients (including cheats) may interfere with the verification process. Since it is the client developer's duty to guarantee vanilla protocol, this cannot be fixed by Sonar.
{% endhint %}

If you have any further questions, please feel free to join the [Discord server](https://jonesdev.xyz/discord) and open a ticket.
