# Recommended Suggester Configuration
Configuring Suggester might not seem simple at first due to the large number of different elements you can currently customize. However, most of these are not mandatory and just exist to give a deeper granularity to server admins wishing to collect their community's feedback. In this guide, we'll go over a few optional elements we recommend you set up for a better experience. Keep in mind none of them is required as this article only serves as a recommendation.

### Anonymous Suggestions
Your members might not always want their identity to be publicily displayed on the suggestion embeds, especially in large server. This is solved by enabling anonymous suggestions which are handled through [slash commands](https://discord.dev/docs/interactions/slash-commands) and give anonimity to the suggester. Don't fear though, this cannot be abused as server staff can see who suggested something for moderation purposes. This is enabled using `.config anon on`.

### Commands Restrictions
This setting might be very important as your server grow. Its purpose is to limit where and which commands can be used. You can simply [set a commands channel](config/commands) which will make the bot send an error message if someone tries to use the beloved `.suggest` command elsewhere. However, there are bad beans out there and thus simply limiting the main command may not be enough. If that's your case, you can decide to completely ["disable" some channels](config/disabledchannels), which will make Suggester kindly ignore any command sent in the configured channels. Last but not least, you can also [disable specific commands](config/disabledcommands) globally (if you don't like big embeds for example).


