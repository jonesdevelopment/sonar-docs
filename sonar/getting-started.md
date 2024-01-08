---
description: Step-by-step guide on how to install Sonar on your server.
---

# Getting started

1. First, download the Sonar jar file.
2. Then, stop your server.
3. Open your server's plugins folder.
4. Drag and drop the Sonar jar file into the plugins folder.
5. Finally, start your server again. Sonar is now protecting your server!

You can [download the latest stable release](https://github.com/jonesdevelopment/sonar/releases/latest) from the [Sonar GitHub repository](https://github.com/jonesdevelopment/sonar/).

<mark style="color:red;">Important:</mark> Please do not upload Sonar to all backend servers if you are using a proxy (BungeeCord or Velocity), as Sonar's anti-bot is supposed to only be executed once for every new connection.

You can also build your own version of Sonar by following the Building guide in the documentation.

{% content-ref url="building.md" %}
[building.md](building.md)
{% endcontent-ref %}

If you have any further questions, join the [Jones Development Discord](https://jonesdev.xyz/discord) and open a ticket or start a discussion thread.
