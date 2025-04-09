# Usage of the config command

The `.config` command allows you to modify how Suggester will work in your server, giving you the ability to customize notifications, permissions, reactions and much more! We'll dive into it later, for now let's talk about the command itself.

?> Looking to quickly setup the bot? Try the [`.setup`](../beginner-guide.md) command instead!

### How can I use it?
To edit a configuration element, use `.config [element] [value]` in any channel the bot can read and send messages in. There are currently 30+ different settings you can customize, which you can find more information on the table below.so we heavily recommand against it.

### Optional Arguments
`.config list` will show the server's current configuration\
`.config [element]` will show the current value of a specific element\
`.config help` with no other argument will show an interactive menu explaining what each element does\
`.config help [element]` will show more information about a specific element

### Aliases
`serverconfig`, `cfg` and `configure`

### Permission
Any member with the **Manage Server** permission or a configured [admin role](/config/adminroles.md) can modify the server configuration.

!> **Warning:** Adding the `@everyone` role as an admin role will give everyone in your server elevated permissions, so we heavily recommend against it.

# Configuration Elements

| Element                                                    | Default Value      | Quick Description¹                                                            |
| ---------------------------------------------------------- | ------------------ | ----------------------------------------------------------------------------- |
| [Admin Roles](/config/adminroles.md)²                      |                    | Roles with all perms                                                          |
| [Allowed Roles](/config/allowedroles.md)                   |                    | Roles allowed to send suggestions                                             |
| [Anonymous Suggestions](/config/anon.md)                   | Disabled           | Settings for anonymous feedback                                               |
| [Approve Role](/config/approverole.md)                     |                    | Roles given to the author of a suggestion when it gets approved               |
| [Autofollowing](/config/autofollowing.md)                  | Enabled            | Settings for autofollowing                                                    |
| [Blocked Roles](/config/blockedroles.md)                   |                    | Roles blocked from sending suggestions                                        |
| [Clean Commands](/config/cleancommands.md)                 | Disabled           | Settings for commands deletion                                                |
| [Color Change](/config/colorchange.md)                     | 15 votes • #FFD700 | Change the color of the suggestion embed when it reaches X net upvotes        |
| [Commands](/config/commands.md)                            |                    | List of channels where commands can be used                                   |
| [Commandless Suggestions](/config/inchannelsuggestions.md) | Disabled           | Settings for commandless suggestion submission                                |
| [Comment Timestamps](/config/ctime.md)                     | Enabled            | Settings for comment timestamps                                               |
| [Cooldown](/config/cooldown.md)                            | None               | Suggestion cooldown                                                           |
| [Denied](/config/denied.md)                                |                    | Channel where denied suggestions are posted                                   |
| [Disabled Channels](/config/disabledchannels.md)           |                    | Channels where commands can't be used                                         |
| [Disabled Commands](/config/disabledcommands.md)           |                    | Disabled commands can't be used                                               |
| [Emojis](/config/emojis.md)                                | 👍,🤷 and 👎      | Reaction emojis to vote on approved suggestions                               |
| [Feed Ping](/config/feedping.md)                           |                    | Role pinged when a suggestion is approved                                     |
| [Implemented](/config/implemented.md)                      |                    | Channel where implemented suggestions are sent                                |
| [Implemented Role](/config/implementedrole.md)             |                    | Role given to the author of a suggestion when it gets marked as Implemented   |
| [Language](/config/locale.md)                              | English            | Server-wide setting for the language used by the bot                          |
| [Live Vote Count](/config/votecount.md)                    | Enabled            | Preferences for vote count                                                    |
| [Logs](/config/logs.md)                                    |                    | Channel where all actions are logged                                          |
| [Mode](/config/mode.md)²                                   |                    | Suggestion handling mode                                                      |
| [Notifications](/config/notify.md)                         | Enabled            | Settings for notifications                                                    |
| [One Vote](/config/onevote.md)                             | Enabled            | Settings to limit voting to only one reaction                                 |
| [Prefix](/config/prefix.md)²                               | `.`                | Symbol to use before commands (eg. `.help`)                                   |
| [Review](/config/review.md)²                               |                    | Channel where pending suggestions are sent                                    |
| [Review Ping](/config/reviewping.md)                       |                    | Role pinged when a new suggestion is submitted                                |
| [Self Vote](/config/selfvote.md)                           | Enabled            | Settings to limit voting on your own suggestions                              |
| [Staff Roles](/config/staffroles.md)²                      |                    | Roles with suggestion managing perms                                          |
| [Suggestion Cap](/config/cap.md)                           | None               | Maximum of concurrent approved suggestions                                    |
| [Suggestions Feed](/config/suggestions.md)²                |                    | Channel where approved suggestions are sent                                   |
| [Voting Roles](/config/voting.md)                          | All roles          | List of roles allowed to vote                                                 |



> ¹ Click on the option name for more information about it!\
² These elements are required for the bot to function properly. If you haven't configured one of those, you'll get a lovely error!

?> [Forum Channels](https://discord.com/blog/forum-channels-space-for-organized-conversation) are not currently supported and may not be set when configuring elements that accept a channel input.
