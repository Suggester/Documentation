# Usage of the config command

The `.config` command allows you to modify how Suggester will interact within your server, you will be able to customize notifications, permissions, reactions and much more! We'll dive into it later, for now let's talk about the command itself

### How can I use it?

To edit a configuration element, use `.config [element] [value]` in any channel the bot can read & send messages in. There are currently 25+ different settings you can customize, which you can find more information on the table below.

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

| Element                                       |  Default Value           |  Quick Description¹  |
|-----------------------------------------------|:------------------------:|------------------------------------------|
| [Admin Roles](/config/adminroles.md)²         |                          | roles with all perms |
| [Allowed Roles](/config/allowedroles.md)      |                          | roles allowed to send suggestions |
| [Approve Role](/config/approverole.md)        |                          | roles given to the author of a suggestion when it gets appproved |
| [Autofollowing](/config/autofollowing.md)     |        Enabled           | settings for autofollowing |
| [Blocked Roles](/config/blockedroles.md)      |                          | roles blocked from sending suggestions |
| [Clean Commands](/config/cleancommands.md)    |       Disabled           | settings for commands deletion |
| [Color Change](/config/colorchange.md)        |   15 votes - #FFD700     | change the color of the suggestion embed when it reaches X net upvotes |
| [Commands](/config/commands.md)               |                          | list of channels where commands can be used | 
| [Comment Timestamps](config/ctime.md)         |       Enabled            | settings for comment timestamps |
| [Cooldown](/config/cooldown.md)               |      0 second            | suggestion cooldown |
| [Denied](/config/denied.md)                   |                          | channel where denied suggestions are posted |
| [Emojis](/config/emojis.md)                   |     👍,🤷 and 👎        | reaction emojis to vote on approved suggestions |
| [Feed Ping](/config/feedping.md)              |                          | role pinged when a suggestion is approved |
| [ICSS](/config/inchannelsuggestions.md)       |       Disabled           | settings for ICSS |
| [Implemented](/config/implemented.md)         |                          | channel where implemented suggestions are sent |
| [Implemented Role](/config/implementedrole.md)|                          | role given to the author of a suggestion when it gets marked as Implemented |
| [Language](/config/locale.md)                 |       English            | the language used by the bot server wide |
| [Logs](/config/logs.md)                       |                          | a channel where all actions are logged |
| [Mode](/config/mode.md)²                      |                          | the suggestion handling mode |
| [Notifications](/config/notify.md)            |       Enabled            | settings for notifications |
| [One Vote](/config/onevote.md)                |       Enabled            | settings to limit voting to one reaction |
| [Prefix](/config/prefix.md)²                  |        `.`               | prefix :bigbrain: |
| [Review](/config/review.md)²                  |                          | review channel where pending suggestions are sent |
| [Review Ping](/config/reviewping.md)          |                          | role pinged when a new suggestion is submitted |
| [Self Vote](/config/selfvote.md)              |       Enabled            | settings to limit voting on owned suggestions |
| [Staff Roles](/config/staffroles.md)²         |                          | roles with suggestion managing perms |
| [Suggestion Cap](/config/cap.md)              |       Infinite           | max of approved suggestions |
| [Suggestions Feed](/config/suggestions.md)²   |                          | channel where approved suggestions are sent |
| [Voting Roles](/config/voting.md)             |      All roles           | list of roles allowed to vote |

> ¹ Click on the option name for more information about it!\
² These elements are required for the bot to function properly, if any of these hasn't been configured, an error will appear.
