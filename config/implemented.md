# Configuration Element: Implemented Suggestions Channel

### Description
The channel where suggestions marked as "Implemented" via the `mark` command are sent. If no channel is configured, implemented suggestions will stay in the suggestions feed.

### Usage
Set up the archive channel using `.config implemented [channel]`, setting `none` as the channel will reset the current configuration.

### Aliases
`archivechannel`, `archive`, `implementedchannel`, `done` and `donechannel`

### Accepted Inputs
Any channel name, id or #mention

?> [Forum Channels](https://discord.com/blog/forum-channels-space-for-organized-conversation) are not currently supported and may not be configured as the implemented suggestions channel.