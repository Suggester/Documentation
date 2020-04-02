# Config
---
### Description
This command is used to set various settings without needing to go through the full setup.
### Optional Arguments
`list` - This argument is used to show current server settings.

`element` - If this is used without any other argument, it will show current settings for that element.




*For configuration*











| Config Element | Function                                                                                                                                                                                                                                                                                             | Valid Inputs                            |                                     Usage                                     |
|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|:-----------------------------------------------------------------------------:|
| admin          | Anyone with this role inherits staff permissions, but also has permission to configure server settings.                                                                                                                                                                                              | Role name, ID, or @mention              | `config admin [add/remove/list] [role]`                                       |
| staff          | Anyone with this role has permission to accept and deny suggestions, as well as interact with them in other ways.                                                                                                                                                                                    | Role name, ID, or @mention              | `config staff [add/remove/list] [role]`                                       |
| review         | The channel where suggestions are sent immediately after submission to be reviewed by staff. (Only if the mode is set to **review**)                                                                                                                                                                 | Channel ID, name or #mention            | `config review [channel]`                                                     |
| suggestions    | The channel where approved suggestions are posted. (If the mode is set to **autoapprove** then suggestions are automatically posted here)                                                                                                                                                            | Channel ID, name or #mention            | `config suggestions [channel]`                                                |
| denied         | The channel where suggestions that are denied/deleted are posted. Using `none` as the channel will remove the denied suggestions channel if there is one set.                                                                                                                                        | Channel ID, name, #mention, or `none`   | `config denied [channel]`                                                     |
| logs           | The channel where all actions taken on suggestions are logged. Using `none` as the channel will remove the log channel if there is one set.                                                                                                                                                          | Channel ID, name, #mention, or `none`   | `config logs [channel]`                                                       |
| emojis         | The emojis that should be reacted on approved suggestions. The defaults are 👍, 🤷, and 👎 for upvote, shrug, and downvote respectively. Selecting `disable` for an emote disables it - meaning it won't be added to new approved suggestions. this is **enabled** by default.                      | Unicode or custom emoji from the server | `config emojis [upvote/shrug/downvote/toggle/enable/disable] [emoji/disable]` |
| notify         | The `notify` element specifies whether server members should be notified through DM when actions are taken on their suggestions. This is **enabled** by default.                                                                                                                                     | `enable`, `disable`, or `toggle`        | `config notify [enable/disable/toggle]`                                       |
| mode           | The `mode` element configures the mode of suggestion handling. Setting this to `review` will put all suggestions through the review process before sending them to the suggestions channel. Setting this to `autoapprove` will automatically send all submitted suggestions to the suggestions feed. | `review` or `autoapprove`               | `config mode [review/autoapprove]`                                            |
| prefix         | The prefix that all commands start with Example: in `.command` the prefix is `.`                                                                                                                                                                                                                     | Any string with no spaces               | `config prefix [prefix]`                                                      |










### Usage
```
.config (element) (additional parameters)
```
### Aliases
`serverconfig`, `cfg`, `configure`
### Required Permissions
People with **Manage Server** permission or configured admin role.