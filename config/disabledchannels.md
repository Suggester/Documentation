# Configuration Element: Disabled Channels

### Description
This setting determines channels where the bot will not respond to any commands

### Usage
Set up disabled channels using `.config disabledchannels add/remove/list [channel]`

### Aliases
`disablechannel`, `disablechannels`, `disabledchannel`, `disablechnl`, `disabledchnl` and `dchnl`

### Accepted Inputs
Any channel name, ID or #mention

!> Disabling the suggestion feed channel will also disable the ability to submit suggestions via any message sent in there, if enabled with [this element](/config/inchannelsuggestions.md).

?> [Forum Channels](https://discord.com/blog/forum-channels-space-for-organized-conversation) are not currently supported and may not be configured as a disabled channel (commands posted in threads or inside forum threads will be ignored).
