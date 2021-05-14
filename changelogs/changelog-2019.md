# Changelog 2019

---
### Suggester v2.1 (November 16th, 2019)
This update brings a lot of cool changes, some of which were suggested by yall! 

- **Setup**: Running the `setup` command will initiate a walkthrough for configuring your server, making it much easier than the config command (which still exists)

- **Permission Checks**: The bot now checks permissions in channels before performing actions, making sure everything works as intended

- **Log Channels**: You can now set a log channel where all actions on suggestions are logged using `.config logs #channel`

- **Removing log and denied suggestions channels**: Specifying `none` as the channel in the `config` command will remove the log or denied suggestions channels 

- **Approve, but with comments**: You can now run `.approve` and specify a comment to add to the suggestion!

- **Attach with uploaded attachments**: You can now upload an attachment straight to Discord for the `attach` command and it will be added to the suggestion

- **Mass approve/deny/delete**: You can now approve/deny/delete multiple suggestions at a time using the `mapprove`, `mdeny`, and `mdelete` commands

- **Enable/disable reactions on the suggestion feed**: You can now toggle whether you would like suggestion feed posts to have reactions with `.config emojis toggle`

- **Enable/disable DMs to server members when suggestions are updated**: Using `.config notifications toggle` will toggle whether server members receive DMs when their suggestions are updated

- **Bug fixes**: Gotta catch 'em all!

 
