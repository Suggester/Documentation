# Configuration Element: Server Locale

### What is it for?
This setting defines which language will Suggester use when responding to commands. If a user has already configured a locale using the `.locale` command, Suggester will prioritize it.

?> If a server has [Community](https://support.discord.com/hc/en-us/articles/360047132851-Enabling-Your-Community-Server) enabled, the bot will attempt to set the configured locale based on the one configured in Community Settings. This process **only** occurs once (when Suggester joins the server).

### Usage
Set up the server locale using `.config locale [language]`

### Aliases
`language`, `lang` and `locales`

### Accepted Imputs
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

?> Interested in translating the bot? Take a look at our [translation program](/topics/community-programs.md)!


