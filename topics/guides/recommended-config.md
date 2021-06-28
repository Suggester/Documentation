# Recommended Suggester Configuration
Configuring Suggester might not seem simple at first due to the large number of different elements you can currently customize. However, most of these are not mandatory and just exist to give a deeper granularity to server admins wishing to collect their community's feedback. In this guide, we'll go over a few optional elements we recommend you set up for a better experience. Keep in mind none of them is required as this article only serves as a recommendation.

### Anonymous Suggestions
Your members might not always want their identity to be publicily displayed on the suggestion embeds, especially in large server. This is solved by enabling anonymous suggestions which are handled through [slash commands](https://discord.dev/docs/interactions/slash-commands) and give anonimity to the suggester. Don't fear though, this cannot be abused as server staff can see who suggested something for moderation purposes. This is enabled using `.config anon on`.

### Commands Restrictions
This setting might be very important as your server grow. Its purpose is to limit where and which commands can be used. You can simply [set a commands channel](config/commands) which will make the bot send an error message if someone tries to use the beloved `.suggest` command elsewhere. However, there are bad beans out there and thus simply limiting the main command may not be enough. If that's your case, you can decide to completely ["disable" some channels](config/disabledchannels), which will make Suggester kindly ignore any command sent in the configured channels. Last but not least, you can also [disable specific commands](config/disabledcommands) globally (if you don't like big embeds for example).

### Feed Reactions
Emojis are great, like for real. Look at [this one](https://cdn.discordapp.com/emojis/830143648679067740.png) for example. Suggester allows you to customize the emojis it adds when a suggestion is approved so people can vote on it and have their voice heard. You can configure any emoji from the current server or the default list, including animated ones. We recommend setting emojis suggesting what they're for, like a green tick for upvotes and a red cross for downvotes. Don't forget the shrug one too ¯\\\_(ツ)\_/¯ \
Check [this page](config/emojis) for more info on customizing these!

### Prefix
Setting a custom prefix is one of the most important things to do when you add a new bot to your server, to avoid receiving 17 DMs when you're just looking for help. Suggester's default prefix is a dot (`.`) but you can change it at anytime to almost anything shorter than 20 characters. You can configure it using `.config prefix [new prefix]`. Who wouldn't like having to use this command? `?]!"{$suggest` 
Please don't use this one though. Like seriously don't, it's ugly. >:(

### Voting Limitations
Suggester currently provides two different settings that relates to voting: `onevote` and `selfvote`. The former prevents members from voting multiple times on the same suggestion (like upvoting and downvoting) and the latter prevents suggestion authors from upvoting their own suggestions, gotta play fair huh. We recommend setting both by respectively using `.config onevote on/off` and `.config selfvote on/off`.

