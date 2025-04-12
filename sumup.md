# Public Commands Sumup
Suggester has a lot of commands that everyone can use, but they don't need their own article as they are quite simple. You'll find in this page a list of public commands with a quick explanation of what they do. Commands in this list will use the default prefix (`.`), which means that if you configured a different one, you will have to replace it accordingly.

### Commands Anyone Can Use

- `.help`: Shows an interactive menu containing all Suggester's commands, can also include a command argument (`.help (command)`) to get info about a specific command.
- `.ping`: Displays the response time and some other information about the bot.
- `.support`: Sends the link to our [support server](https://suggester.js.org/support) where you can get in touch with our Support Team.
- `.invite`: Sends the link to [add the bot](https://suggester.js.org/invite) to your server.
- `.verify`: Shows a user permissions as they relate to the bot, also accepts a mention/user id argument to check someone else's permissions.
- `.prefix`: Shows the currently configured prefix in the server.
- `.tutorial`: Shows a quick guide about setting up and using the bot (the response to this command is the same as the embed sent when the bot is added to a server)
- `.github`: Links Suggester's repository, where you can contribute to its development!
- `.shard`: Tells which group of servers the current server is part of. 
- `.legal`: Sends the link to our [privacy policy](/legal/privacy.md).

## Special Sunflowers

These are special commands everyone can use, so we added them to another section :)

- `.notify`: Defines your notification settings for the current server, running this command with no argument will show your current settings. Add `on` or `off` to change your preferences.
  
- `.suggest`: Suggester's main command! Use it to suggest stuff in your favorite servers, you can also add an attachment by attaching it to the command message! Each suggestion can contain up to 1,900 characters.

- `.locale`: This command sets your **user** locale, all responses and messages you receive from the bot will use that language (defaulting to English). Using it with no arguments will show a list of all available locales.

?> If you've configured a language and the bot still responds in English, it means this specific string has not yet been translated.

- `.shortinfo`: This command has its own article which you can read [here](topics/shortinfo.md).

### Commands Available in DMs
The following commands are available in direct messages with Suggester:

`ping`, `follow auto`, `follow list`, `notify` and `privacy`

## Suggestion Following

### What is that?
You can follow suggestions to be notified when a change is made to them. It works just like normal notifications, but the title refers to "a suggestion you follow" instead of "your suggestion". You can follow suggestions using the [`.follow`](topics/follow.md) command, or by upvoting them: you will receive a DM the first time you upvote a suggestion which will contain basic information about auto-following.

### Auto-following 
By default, you'll automatically follow suggestions when you **upvote** them, though that can be disabled using `.follow auto off`, which means you will not receive notifications for suggestions you've auto-followed in the past, and you won't follow any more automatically. If you turn it back on, you'll receive notifications again for suggestions you auto-followed. Servers admins can also choose to disable auto-following! Check this [page](/config/autofollowing.md) for more information.  