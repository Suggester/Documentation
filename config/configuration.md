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
| [Admin Roles](/config/adminroles)             | Role                                         |        ✓              |      None               |
| [Allowed Roles](/config/allowedroles.md)      | Role                                         |                       |         None              | 
| [Approve Role](/config/approverole.md)        | Role                                         |                       |         None              |
| [Blocked Roles](/config/blockedroles.md)      | Role                                         |                       |         None              |
| [Clean Commands](/config/cleancommands.md)    | Toggle                                       |                       |         Disabled              |
| [Color CHange](/config/colorchange.md)        |                                              |                       | 15 votes - #FFD700     |
| [Commands](/config/commands.md)               | Channel                                      |                       |         None              |
| [Cooldown](/config/cooldown.md)               | Number                                       |                       |       0 seconds                |
| [Denied](/config/denied.md)                   | Channel                                      |           ✓           |         None              |
| [Emojis](/config/emojis.md)                   | Emojis                                       |                       |          👍,🤷 and 👎             |
| [Implemented](/config/implemented.md)         | Role                                         |                       |        None               |
| [ICSS](/config/inchannelsuggestions)          | Toggle                                       |                       |         Disabled              |
| [Locale](/config/locale.md)                   | Role                                         |                       |          English             |
| [Logs](/config/logs.md)                       | Channel                                      |                       |            None           |
| [Mode](/config/mode.md)                       |                                              |           ✓            |            None          |
| [Notifications](/config/notify.md)            |  Toggle                                      |                       |            Enabled           |
| [One Vote](/config/onevote.md)                |  Toggle                                      |                       |                       |
| [Ping Role](/config/pingrole.md)              | Role                                         |                       |   None                    |
| [Prefix](/config/prefix.md)                   |                                              |          ✓             |     `.`                  |
| [Review](/config/review.md)                   | Channel                                      |          ✓             |     None                  |
| [Self Vote](/config/selfvote.md)              | Toggle                                       |                       |                                |
| [Staff Roles](/config/staffroles.md)          | Role                                         |           ✓            |       None                      |
| [Suggestions](/config/suggestions.md)         | Channel                                      |          ✓             |       None                      |
| [Voting Roles](/config/voting.md)             | Role                                         |                        |       All roles                  |

\* The `Required?` colon denotes if each element is required or not for the bot to function properly


