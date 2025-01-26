---
description: Supported languages in Sonar
---

# Translations

Currently supported languages:

* English - by [Jones](https://github.com/jonesdevelopment) - `en`
* Dutch - by [Jones](https://github.com/jonesdevelopment) - `nl`
* German - by [micartey](https://github.com/micartey) - `de`
* Czech - by [slosa](https://github.com/slosacoder) - `cs`
* French - by ekiff - `fr`
* Turkish - by [Jenkins](https://github.com/ayazjenkins) - `tr`
* Polish - by Najek, foren - `pl`
* Russian - by MISHA, Null - `ru`
* Spanish - by Juansitoh - `es`&#x20;
* Indonesian - by [LourenT](https://github.com/LOURENT4462) - `id`
* Georgian - by [GreenedDev](https://github.com/GreenedDev), [Chumb3x](https://github.com/chumb3x) - `ka`
* Simplified Chinese - by [FallenCrystal](https://github.com/fallencrystal) - `zh`
* Brazilian Potuguese - by [RenanGabrieel](https://github.com/RenanGabrieel) - `pt-br`

In order to use a language, you need to modify the `language.properties` file in Sonar or change your system language. If you let Sonar regenerate the files (e.g., by deleting them and restarting the server), the new language will be automatically used for the translations.

### Manual migration

If you want to manually migrate your language files, you can find all the translated files on GitHub. Simply choose the type of translation (configuration, messages, or webhook configuration) and select the language you want to use in Sonar. Then, you can copy or replace your current file(s) with the file you want to use.

If you are interested in contributing new translations, please do so via a GitHub Pull Request. If you have any further questions, please feel free to join the [Discord](https://jonesdev.xyz/discord) and open a ticket.
