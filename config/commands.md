# Configuration Element: Commands Channel

### Description
This setting defines what channels can the `.suggest` command be used in.

### Usage
Set up commands channels using `.config commands add/remove/list [channel]`, setting `none` as the channel will reset the current configuration and thus will allow the command to be used in any channel

### Aliases
`commandchannels`, `command`, `commandchannel` and `commands`

### Accepted Inputs
Any channel name, ID or #mention

?> [Forum Channels](https://discord.com/blog/forum-channels-space-for-organized-conversation) are not currently supported and may not be configured as a command channel (commands posted in threads or inside forum threads will be ignored).