---
description: Supported languages in Sonar
---

# Translations

You can view a full list of valid language codes on [Wikipedia](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes).

Currently supported languages:

* English - by [Jones](https://github.com/jonesdevelopment) - `en`
* Russian - by [MISHA](https://github.com/f3f5), Null - `ru`
* Polish - by Najek, foren - `pl`
* French - by ekiff - `fr`
* German - by [micartey](https://github.com/micartey) - `de`
* Dutch - by [Jones](https://github.com/jonesdevelopment) - `nl`
* Czech - by [slosa](https://github.com/slosacoder) - `cs`
* Georgian - by [GreenedDev](https://github.com/GreenedDev), [Chumb3x](https://github.com/chumb3x) - `ka`
* Chinese Simplified - by [FallenCrystal](https://github.com/fallencrystal) - `zh`
* Spanish - by Juansitoh - `es`  (`config.yml` missing)
* Indonesian - by [LourenT](https://github.com/LOURENT4462) - `id`  (`config.yml` missing)
* Turkish - by [Jenkins](https://github.com/ayazjenkins) - `tr`  (`config.yml` and `webhook.yml` missing)

In order to use a language, you need to modify the `language.properties` file in Sonar or change your system language. If you let Sonar regenerate the files (e.g., by deleting them and restarting the server), the new language will be automatically used for the translations.

### Manual migration

If you want to manually migrate your language files, you can find all the translated files on GitHub. Simply choose the type of translation (configuration, messages, or webhook configuration) and select the language you want to use in Sonar. Then, you can copy or replace your current file(s) with the file you want to use.

If you are interested in contributing new translations, please do so via a GitHub Pull Request.
