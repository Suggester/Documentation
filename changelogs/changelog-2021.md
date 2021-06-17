# Changelog 2021
---
### Suggester v4.10.3 (June 17th, 2021)
• The `.edit` command should work properly now
• Announcement channels are now supported for channel configuration
• Minor fixes to the `top` and `down` commands

### Suggester v4.10.2 (May 26th, 2021)
This release aims to mitigate issues where suggestions submitted (generally on the autoapprove mode) would appear in the suggestions feed as completely different suggestions. 
Please contact our [support team](https://suggester.js.org/support) if this issue still occurs! 

### Suggester v4.10.1 (May 13th, 2021)
Discord has [rebranded](https://dis.gd/ournewlook), changing their old blurple color (#7289DA) to a new brighter blue (#5865F2). Since Suggester's profile picture and default color scheme used the OG Blurple color, we're rebranding our icons and assets as well. You'll notice a brand new Suggester icon, as well as a new default color for suggestion embeds and some emojis used by the bot. And happy birthday Discord!!

### Suggester v4.9.10 (April 15th, 2021)

**New Things**\
• Commands can now be disabled server-wide using `.config disabledcommands [add/remove] [command name]`\
• Channels can now be disabled, meaning the bot will not respond to any commands in that channel. This is done using `.config disabledchannels [add/remove] [#channel]`\
• The `privacy` command has been added, linking to our privacy policy.

**Improvements**\
• The prefix can now be edited using the `.prefix` command directly. This is done using `.prefix [your new prefix here]`

**Bug Fixes**\
• Blocked users can no longer use `/asuggest`\
• Comments added through the `.mark` command are no longer duplicated

**Removed**\
• The `.stats` command was removed because the information it provided was outdated

### Suggester v4.1.2021 (April 1st, 2021)
Suggester v4.1.2021 is the largest overhaul Suggester has ever had. We coded until our fingers couldn't anymore, and then we started using our toes. This update contains major updates to our patented SuggestionCreator3000™, allowing for even better-er suggestion creation. The bot also now runs 0% faster, and uses 500% more memory (meaning it will remember your suggestions better... yay!) 

...and it now has owo mode
thank you for your time and have a good day

If you hate owo mode you can use `.locale eng` to go back to English but everyone will judge you for it! 

---
### Suggester v4.9.1 (March 29th, 2021)
- The live vote count on suggestions can now be hidden using `config votecount off`
- When the `autoapprove` mode is set, the response to the `deny` command will now mention the `delete` command
- The bot now responds with the prefix if the message is just the bot mention
- If a server is set as a Community on Discord and has a locale set in Server Settings, the bot will try to find that locale and set it as the configured locale on the bot 

---
### Suggester v4.9 (March 23rd, 2021)
🆕 **New Things**
- Added the `shards` command to show information about all bot shards
- Added the `search` command, which takes an unlimited number of query parameters, space-separated to query all suggestions on the server. See this [page](topics/search.md) for more information.

🔧 **Improvements**
- The emojis used in the `mark` command are now colorblind-friendly
- You can now add attachments to suggestions awaiting review through the `attach` command
- The `info` command now shows a timestamp for when the suggestion was submitted
- There is now an error message shown when trying to set the `cooldown` config element lower than the global cooldown for the `suggest` command
- The denial reason is now shown in the review message when "A change has been processed on this suggestion" is shown
- The `setup` command now links to the documentation for each config element
- Using `default` as the emoji setting will restore a reaction to its default configuration
- `dupe` can now be used on approved suggestions, deleting them from the suggestions feed

🐛  **Bug Fixes**
- The `help` command is no longer available in DMs
- Anonymous suggestions now properly handle allowed roles configuration and checking
- Anonymous suggestions will now show as anonymous in the denied suggestions feed
- Missing upvote/downvote reactions should no longer cause issue with live vote totals and `colorchange` config

---
### Suggester v4.7.2 (January 31st, 2021)
- The `ping` command has been redesigned to show more information and not error when the bot is starting up
- The `mark` command should no longer output an error if you don't specify a status in the command and select a reaction to choose one
- Voting totals (upvotes/downvotes) should be more accurate now
- **@everyone** and **@here** mentions for the `feedping` and `reviewping` elements now resolve correctly and ping intended users


---
### Suggester v4.7.1 (January 6th, 2021)
- We now support importing suggestions from the `Gaius Cicereius#3705` bot
- You can now enable/disable comment timestamps on the suggestion embeds using `cfg commenttime [on/off/toggle]` 

---
### Suggester v4.7 (January 4th, 2021)
- This release brings a new major feature to the bot: a Trello integration! We have a new documentation page for it, which can be found [here](/topics/trello/intro.md), and you can also use `config help trello` to find more examples
- The `queue` command now shows the suggestions you are viewing out of the whole in the title (ex. 1-10 out of 20)
- `shortinfo` now has options to shorten the output:\
Adding `-trimsuggest` (or `-ts` for short) to the end will limit the suggestion content output to 250 character\
Adding `-noattach` (`-na` for short) will hide the suggestion's attachment
- Added suggestion caps: these prevent more suggestions from being submitted if the number of approved, non-denied, non-implemented suggestions is greater than or equal to the amount configured using `config cap`
- Command-specific documentation links can now be found in `help [command]`, as well as in `config help [element]`
- Added the feed ping role: when a suggestion is sent to the suggestions feed via autoapprove or manual approval the role will be mentioned. This role can be configured using `config feedping`. Due to there now being 2 ping roles, the old `pingrole` is now called `reviewping`
- Messages from blocked users are now deleted when `inchannelsuggestions` is enabled
- `autosetup` channel names now reflect guild locale-specific configuration
- Servers with over 5000 members may receive a large server protip
- `in` was removed as an alias for  the "in progress" status
- Global cooldown messages will now be affected by server `cleancommands` configuration
- Minor bugfixes and improvements
