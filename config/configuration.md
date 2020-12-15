# Usage of the config command

The `.config` command allows you to modify how Suggester will interact within your server, you will be able to customize notifications, permissions, reactions and more! We'll dive into it later, for now let's talk about the command itself.

### How can I use it?

To edit a configuration element, use `.config [element] [value]` in any channel the bot can read & send messages in. There are currently 25+ different settings you can customize, which you can find more information on the table below.

### Optional Arguments

`.config list` will show the server's current configuration & its status.\
`.config [element]` will show the current value of a specific element.\
`.config help` with no other argument will show an interactive menu explaining all elements like in this documentation.\
`.config help [element]` will show more information about a specific element.

### Aliases
`serverconfig`, `cfg` and `configure`

### Permission
Any member with the **Manage Server** permission or a configured [admin role](/config/adminroles.md) is able to modify the server configuration.

!> **Warning:** Adding the `@everyone` role as an admin role will give everyone in the server elevated permissions and may cause harm, do it at your own risks!

# Configuration Elements

| Element                                       |  Default Value          |  Quick Description¹  |
|-----------------------------------------------|:------------------------:|------------------------------------------|
| [Admin Roles](/config/adminroles.md)²         |                     | The roles with all permissions. |
| [Allowed Roles](/config/allowedroles.md)      |               | The roles allowed to send suggestions. |
| [Approve Role](/config/approverole.md)        |                       | The roles given to the author of a suggestion when it gets appproved. |
| [Approved Suggestions](/config/approvedsuggestions.md)²  |            |  The channel where approved suggestions are sent to. |
| [Autofollowing Preferences](/config/autofollowing.md) |      Enabled        | The settings for autofollowing a suggestion. |
| [Blocked Roles](/config/blockedroles.md)      |                     | The roles blocked from sending suggestions. |
| [Clean Commands](/config/cleancommands.md)    |           Disabled       | The settings for commands deletion. |
| [Color Change](/config/colorchange.md)        |   15 votes - #FFD700     | To change the color of the suggestion embed when it reaches X net upvotes. |
| [Commands](/config/commands.md)               |                    | The list of channels where commands can be used. | 
| [Cooldown](/config/cooldown.md)               |      0 second         | The suggestion cooldown. |
| [Denied](/config/denied.md)                   |                  | The channel where denied suggestions are posted. |
| [Emojis](/config/emojis.md)                   |   👍,🤷 and 👎     | The reaction emojis to vote on approved suggestions |
| [ICSS](/config/inchannelsuggestions.md)       | Disabled       | The settings for ICSS (Inchannel Suggestions). |
| [Implemented](/config/implemented.md)         |               | The channel where implemented suggestions are sent to. |
| [Implemented Role](/config/implementedrole.md)|                   | The role given to the author of a suggestion when it gets marked as [Implemented](/config/implemented.md). |
| [Language](/config/locale.md)                 |       English       | The language used by the bot server wide. |
| [Logs](/config/logs.md)                       |                   | A channel where all actions are logged. |
| [Mode](/config/mode.md)²                       |               | The suggestion handling mode ([Autoapproval](/config/mode.md) or [review](/config/review.md)). |
| [Notifications](/config/notify.md)            |           Enabled     | The settings for notifications. |
| [One Vote](/config/onevote.md)                |  Enabled          | The settings to limit voting to one reaction. |
| [Ping Role](/config/pingrole.md)              |                   | The role pinged when a new suggestion is submitted. |
| [Prefix](/config/prefix.md)²                   |       `.`               | The prefix :bigbrain:. |
| [Review](/config/review.md)²                   |                   | The review channel where pending suggestions are sent. |
| [Self Vote](/config/selfvote.md)              |  Enabled         | The settings to limit voting on own suggestions. |
| [Staff Roles](/config/staffroles.md)²          |               | The roles with suggestion managing perms. |
| [Voting Roles](/config/voting.md)            |      All roles         | The list of roles allowed to vote. |

> ¹ Click on the option link for more information about it!\
² These elements are required for the bot to function properly, if any of these hasn't been configured, an error will appear.
