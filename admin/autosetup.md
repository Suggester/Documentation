# Command: autosetup
---
### What does it do?
This command allows admins to automatically setup the bot. This will automatically create four channels, one for [approved suggestions](/config/suggestions.md), one for [denied suggestions](/config/denied.md), one for [pending suggestions](/config/review.md) and one for [logs](/config/logs.md). If you are looking for more granular options, take a look at the [setup](/admin/setup.md) and [config](config/configuration.md) commands.

### Usage
Run `.autosetup` in any channel the bot can read and send messages in

### Alias
`.autoconfig`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [admin](/config/adminroles.md) role

### Bot Permission
To execute this command, Suggester will need the **Manage Channels** permission

![manage channels permission](https://cdn.discordapp.com/attachments/769650556502409226/794313355606097950/unknown.png)

?> Channel names now use the guild's configured [language](/config/locale.md), though only if the corresponding string have been translated.
