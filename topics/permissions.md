### What permissions does Suggester need and why?

When you click on the link to invite the bot, you'll be prompted to confirm that you want to give certain permissions to the bot. If you're skeptical about giving permissions (which is okay!), you might not want to give them, especially elevated ones, without knowing why the bot needs it. We'll explain below why does Suggester ask for each permission and if it is required or not.

### Optional Permissions

**Manage Roles**: Certain configuration elements allow you to reward users with a role when their suggestion is approved or marked as implemented\
**Manage Channels**: If you want the bot to configure itself automatically, you can run the `.autosetup` command which will create a few useful channels in your server, more info [here](admin/autosetup.md)\
**Manage Webhooks**: You can configure a channel where all Suggester-actions will be logged. To avoid rate limits issues, the bot will create a webhook called "Suggester Logs" and post in the configured logging channel\
**Manage Messages**: The `cleancommands` configuration element makes the bot automatically remove both the command and the response message after a few seconds, the permission is required to delete the command message as it was sent by someone else

### Required Permissions
**Read Messages & Read Message History**: Suggester needs to be able to read users' messages to detect when a command is used or when someone sends a message in the suggestions feed while the `sendinchannel` configuration element is enabled\
**Send Messages**: This permission is required for the bot to respond to commands, you don't want to be ignored right??\
**Embed Links**: This allows the bot to send messages with rich embeds, because the colored bar is a blast\
**Add Reactions**: Approved suggestions can be voted on by using specific reactions added by the bot when the suggestion is approved\
**Use External Emojis**: Suggester uses custom made emojis for certain commands (like `.mark` or `.config list`)
