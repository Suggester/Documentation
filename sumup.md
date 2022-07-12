# Public Commands Sumup
Suggester contains a lot of commands everyone can use, but they don't really need a whole article for each and every of them, as they are mostly basic. You'll find in this page the full list of public commands with a quick explanation of what they do. Commands in this list will use the default prefix (`.`), meaning if you configured a different one, you will have to replace it accordingly.

### Commands Anyone Can Use

- `.help`: Shows an interactive menu containing all Suggester's commands, can also include a command argument (`.help (command)`) to get info about a specific command.
- `.ping`: Displays the response time and some other information about the bot.
- `.support`: Sends the link to our [support server](https://suggester.js.org/support) where you can get in touch with our Support Team.
- `.invite`: Sends the link to [add the bot](https://suggester.js.org/invite) to your server.
- `.vote`: Displays information about [voting](topics/supporting.md) for Suggester on several bot listing websites.
- `.verify`: Shows a user permissions as they relate to the bot, also accepts a mention/user ID argument to check someone else's permissions.
- `.prefix`: Shows the current configured prefix in your server.
- `.changelog`: Links the latest stable release from [GitHub](https://github.com/Suggester/Suggester/releases/latest)
- `.tutorial`: Shows a quick guide about setting up and using the bot (the response to this command is the same as the embed sent when the bot is added to a server)
- `.github`: Links Suggester's repository, where you can contribute to its development!
- `.shard`: Tells which shard the current server is on. [Learn more](https://discord.com/developers/docs/topics/gateway#sharding)
- `.shards`: Displays some statistics about the bot's shards.
- `.legal`: Sends the link to our [privacy policy](/legal/privacy.md).

## Special Sunflowers

These are special commands everyone can use, so we added them to another section :)

- `.notify`: Defines your notification settings for the current server, running this command with no argument will show your current settings. To edit them, you'll need an extra argument as shown below:

| Argument           | Description                               |
|--------------------|:-----------------------------------------:|
| `on`               | Enable notifications                      |
| `off`              | Disable notifications                     |
| `toggle`           | Switch to the other state                 |
  
- `.suggest`: Suggester's main command! Use it to suggest stuff in your favorite servers, you can also add an attachment by attaching it to the command message! Each suggestion can contain up to 1900 characters.

- `.locale`: This command sets your **user** locale, all responses and messages you receive from the bot will use that language (defaulting to English). Using it with no arguments will show a list of all available locales.

?> Translations are community made, meaning all locales might not be fully translated when you see them in the bot. If you've configured a language and it responds in English, it means this specific string was not yet translated. More info about community translations can be found [here](community-programs?id=🌐-translating-suggester). 

- `.shortinfo`: This command has its own article which you can see [here](topics/shortinfo.md)

### Commands Available in DMs
The following commands are available in direct messages with Suggester:

`ping`, `changelog`, `follow`, `notify` and `privacy`

## Suggestion Following

### What is that?
You can follow suggestions to be notified when a change is made to them. It works just like normal notifications, but the title refers to "a suggestion you follow" instead of "your suggestion". You can follow suggestions using the [`.follow`](topics/follow.md) command, or by upvoting them: you will receive a DM the first time you upvote a suggestion which will contain basic information about autofollowing.

### Autofollowing 
By default, you'll automatically follow suggestions you **upvote**, though that can be disabled using `.follow auto off`, which means you will not receive notifications for suggestions you've autofollowed in the past, and you won't follow any more automatically. If you turn it back on, you'll receive notifications again for suggestions you autofollowed. This respects all server and user notification settings.
Servers admins can also choose to disable autofollowing! See this [element](/config/autofollowing.md) for more information.  
