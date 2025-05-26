# Configuration Element: Logs Channel

### Description
The channel where every suggestion-managing related actions are logged, see below for a list of logged actions.

### Usage
Set up the logs channel using `.config logs [channel]`, setting `none` as the channel will reset the current configuration

?> Suggester will create a [webhook](https://support.discord.com/hc/en-us/articles/228383668) called "Suggester Logs" in the configured channel. Make sure the bot can both view the channel **and** manage webhooks there!

### Aliases
`logs`, `logchannel` and `logschannel`

### Accepted Inputs
Any channel name, id or #mention

### Logged Actions
- Suggestion approvals, denials, deletions and submissions
- [Anonymous suggestions](/topics/anonymous-suggestions.md)
- Comments (both public and [anonymous](/staff/acomment.md)) and their [deletion](/staff/deletecomment.md)
- Status changes
- Blocks & unblocks
- Attachments added with the [`.attach`](/staff/attach.md) command
- [Edition and edition requests](editing/suggestion-editing.md) and their [approval](editing/approveedit.md) or [denial](editing/denyeedit.md)

?> [Forum Channels](https://discord.com/blog/forum-channels-space-for-organized-conversation) are not currently supported and may not be configured as the logging channel.