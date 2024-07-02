---
description: Supported languages in Sonar
---

# Translations

You can view a full list of valid language codes on [Wikipedia](https://en.wikipedia.org/wiki/List\_of\_ISO\_639\_language\_codes).

Currently supported languages:

* English - `en`
* Russian - `ru`
* French - `fr`
* Dutch - `nl`
* Chinese Simplified - `zh`
* Spanish - `es` (`config.yml` missing)
* Indonesian - `id` (`config.yml` missing)
* Czech - `cs` (`messages.yml` missing)
* Georgian - `ka` (`messages.yml` missing)
* Turkish - `tr` (`config.yml` and `webhook.yml` missing)

In order to use a language, you need to modify the `language.properties` file in Sonar or change your system language. If you let Sonar regenerate the files (e.g., by deleting them and restarting the server), the new language will be automatically used for the translations.

### Manual migration

If you want to manually migrate your language files, you can find all the translated files on GitHub. Simply choose the type of translation (configuration, messages, or webhook configuration) and select the language you want to use in Sonar. Then, you can copy or replace your current file(s) with the file you want to use.
