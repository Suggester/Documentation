# Usage of the config command

The `.config` command allows you to modify how Suggester will interact within your server, you will be able to customize notifications, permissions, reactions and much more! We'll dive into it later, for now let's talk about the command itself.

### How can I use it?

To edit a configuration element, use `.config [element] [value]` in any channel the bot can read & send messages in. There are currently 20+ different settings you can customize, which you can find more information on the table below.

### Optional Arguments

`.config list` will show the server's current configuration & its status\
`.config [element]` will show the current value of a specific element\
`.config help` with no other argument will show an interactive menu explaining all elements like in this documentation\
`.config help [element]` will show more information about a specific element

### Aliases
`serverconfig`, `cfg` and `configure`

### Permission
Any member with the **Manage Server** permission or a configured [admin role](/config/adminroles.md) is able to modify the server configuration

!> **Warning:** Adding the `@everyone` role as an admin role will give everyone in the server elevated permissions and may cause harm, do it at your own risks!

# Configuration Elements

| Element                                       |                Type                          |   Required?¹          | Default Value          |
|-----------------------------------------------|:--------------------------------------------:|-----------------------|------------------------|
| [Admin Roles](/config/adminroles.md)          | Role                                         |        ✓              |         None           |
| [Allowed Roles](/config/allowedroles.md)      | Role                                         |                       |         None           | 
| [Approve Role](/config/approverole.md)        | Role                                         |                       |         None           |
| [Autofollowing Preferences](/config/autofollowing.md) | Toggle                               |                       |         Enabled        |
| [Blocked Roles](/config/blockedroles.md)      | Role                                         |                       |         None           |
| [Clean Commands](/config/cleancommands.md)    | Toggle                                       |                       |         Disabled       |
| [Color Change](/config/colorchange.md)        |                                              |                       | 15 votes - #FFD700     |
| [Commands](/config/commands.md)               | Channel                                      |                       |         None           |
| [Cooldown](/config/cooldown.md)               | Number                                       |                       |       0 second         |
| [Denied](/config/denied.md)                   | Channel                                      |                       |         None           |
| [Emojis](/config/emojis.md)                   | Emojis                                       |                       |      👍,🤷 and 👎     |
| [ICSS](/config/inchannelsuggestions.md)       | Toggle                                       |                       |         Disabled       |
| [Implemented](/config/implemented.md)         | Role                                         |                       |        None            |
| [Implemented Role](/config/implementedrole.md)| Role                                         |                       |        None            |
| [Language](/config/locale.md)                 | Role                                         |                       |          English       |
| [Logs](/config/logs.md)                       | Channel                                      |                       |            None        |
| [Mode](/config/mode.md)                       |                                              |           ✓           |            None       |
| [Notifications](/config/notify.md)            |  Toggle                                      |                       |            Enabled     |
| [One Vote](/config/onevote.md)                |  Toggle                                      |                       |       Enabled          |
| [Ping Role](/config/pingrole.md)              | Role                                         |                       |   None                 |
| [Prefix](/config/prefix.md)                   |                                              |          ✓             |     `.`               |
| [Review](/config/review.md)                   | Channel                                      |          ✓             |     None              |
| [Self Vote](/config/selfvote.md)              | Toggle                                       |                       |         Enabled         |
| [Staff Roles](/config/staffroles.md)          | Role                                         |           ✓            |       None             |
| [Suggestions Feed](/config/suggestions.md)    | Channel                                      |          ✓             |       None             |
| [Voting Roles](/config/voting.md)             | Role                                         |                        |       All roles         |

¹ The `Required?` colon denotes if each element is required or not for the bot to function properly, not configuring required elements will show an error


