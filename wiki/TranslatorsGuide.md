# Translators Guide for RotU

**Applies to:** RotU 2.2 and later

## Introduction

This document provides guidance for anyone working to translate RotU project resources into languages other than English.

## Credentials

To update or create translations for the project, you will need write access to the repository.  
If you want to help translate RotU, please send me an email.

## Subversion Checkout

To begin translating:

1. Checkout a **read-write** copy of the repository head, as described in the **[Setting Up a Development Environment](DevelopmentEnvironment.md)** guide.
2. You do **not** need to set up a full development/build environment — just the source code is sufficient.

## Translating Wiki Pages \*\*\*DEPRECATED\*\*\*

For an overview of how wiki translation works, see:  
[Localizing Wiki Content](http://code.google.com/p/support/wiki/WikiSyntax#Localizing_Wiki_Content)

Once you commit your translated wiki page to the repository, the wiki will automatically serve the translated version to users whose browser language matches the translation.  
If no translated page exists for their language, it will fall back to the English version.

## Translating Configuration Files

The `*.cfg` files contain documentation and default strings that should be translated.

**Rules:**

- Translated config files must keep the **exact same filename** as the original.
- Place them in the appropriate language folder under the `i18n` directory.

**Example (Spanish):**
- Original: `server_default.cfg`
- Translated: `i18n/es/config/server_default.cfg`

> **Note:** `i18n` stands for **internationalization**.  
> Language folders use the standard **2-character ISO-639 language codes** (e.g. `es` for Spanish, `fr` for French, `de` for German, etc.).

### What to Translate

In the configuration files, **do NOT** translate:

- Dvar names (e.g. `sv_mapvoting1`, `game_assistance_enabled`, etc.)

**Do translate:**

- Comments and documentation
- Default strings (especially "Did You Know" messages)
- Any user-facing text

---

*Originally ported from the Google Code wiki.*