# Configuration Element: Server Locale

### Description
This setting defines which language Suggester will use when responding to commands. If a user has already configured a locale using the `.locale` command, it will be prioritized.

?> If a server has [Community](https://support.discord.com/hc/en-us/articles/360047132851) enabled, the bot will attempt to set the configured locale to the one configured in Community Settings. This process **only** occurs once when Suggester joins the server.

### Usage
Set up the server locale using `.config locale [language]`

### Aliases
`language`, `lang` and `locales`

### Accepted Inputs
A supported locale name or code, which you can find using `.locales`

### Completed Locales Right Now
The following locales are completely translated at the moment:

- English (en)
- Greek (el)
- Spanish (es)
- French (fr) 
- Italian (it)
- Dutch (nl)
- Brazilian Portuguese (pt-br)