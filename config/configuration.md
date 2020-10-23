# Usage of the config command

The `.config` command allows you to modify how Suggester will interact within your server, you will be able to customize notifications, permissions, reactions and much more! We'll dive into it later, for now let's talk about the command itself.

### How can I use it?

To edit a configuration element, use `.config [element] [value]` in any channel the bot can read & send messages in. There are currently 20+ different settings you can customize, which you can find more information on the table below.

### Optional Arguments

`.config list` will show the current configuration & its status\
`.config [element]` will show the current value of a specific element\
`.config help` with no other argument will show an interactive menu explaining all elements like this documentation\
`.config help [element]` will show more information about a specific element

### Aliases
`serverconfig`, `cfg` and `configure`

### Permission
Any member with the **Manage Server** permission or a configured admin role is able to modify the server configuration

⚠ **Warning:** Adding the `@everyone` role as an admin role will give everyone in the server elevated permissions and may cause harm, do it at your own risks!

# Configuration Elements
/config/


| Element                                       |                Type                          |   Required?*          | Default Value         |
|-----------------------------------------------|:--------------------------------------------:|-----------------------|-----------------------|
| [Admin Roles](/config/adminroles)             | Role                                         |                       |                       |
| [Allowed Roles](/config/allowedroles.md)      | Role                                         |                       |                       | 
| [Staff Roles](/config/staffroles.md)          | Role                                         |                       |                       |
| [Approve Role](/config/approverole.md)        | Role                                         |                       |                       |
| [Blocked Roles](/config/blockedroles.md)      | Role                                         |                       |                       |
| [Clean Commands](/config/cleancommands.md)    | Role                                         |                       |                       |
| [Color CHange](/config/colorchange.md)        | Role                                         |                       |                       |
| [Commands](/config/commands.md)               | Role                                         |                       |                       |
| [Cooldown](/config/cooldown.md)               | Role                                         |                       |                       |
| [Denied](/config/denied.md)                   | Role                                         |                       |                       |
| [Emojis](/config/emojis.md)                   | Role                                         |                       |                       |
| [Implemented](/config/implemented.md)         | Role                                         |                       |                       |
| [ICSS](/config/inchannelsuggestions)          | Role                                         |                       |                       |
| [Locale](/config/locale.md)                   | Role                                         |                       |                       |
| [Logs](/config/logs.md)                       | Role                                         |                       |                       |
| [Mode](/config/mode.md)                       | Role                                         |                       |                       |
| [Notifications](/config/notify.md)            | Role                                         |                       |                       |
| [One Vote](/config/onevote.md)                | Role                                         |                       |                       |
| [Ping Role](/config/pingrole.md)              | Role                                         |                       |                       |
| [Prefix](/config/prefix.md)                   | Role                                         |                       |                       |
| [Review](/config/review.md)                   | Role                                         |                       |                       |
| [Self Vote](/config/selfvote.md)              | Role                                         |                       |                       |
| [Staff Roles](/config/staffroles.md)          | Role                                         |                       |                       |
| [Suggestions](/config/suggestions.md)         | Role                                         |                       |                       |
| [Voting Roles](/config/voting.md)             | Role                                         |                       |                       |


