---
description: Why Sonar uses adventure's MiniMessage
---

# Usage of MiniMessage

Sonar uses [MiniMessage](https://docs.advntr.dev/minimessage/) formatting, as this allows administrators to fully customize all messages to their hearts content. By using MiniMessage in Sonar, administrators are able to use fully custom [colors](https://docs.advntr.dev/minimessage/format.html#color), [click events](https://docs.advntr.dev/minimessage/format.html#click), [hover events](https://docs.advntr.dev/minimessage/format.html#hover), and [more](https://docs.advntr.dev/minimessage/format.html).

* You can find a live MiniMessage component preview in the [MiniMessage Viewer](https://webui.advntr.dev/).
* You can find Sonar's translations in the `messages.yml` file in the plugin directory.
* The MiniMessage formatting does not only apply to chat messages but also to action bars, titles, and disconnect messages. However, some events might not always be supported (for example, you are unable to create a hover or click event in a disconnect message, title, and action bar).

If you have any further questions, please feel free to join the [Discord server](https://jonesdev.xyz/discord) and open a ticket.
