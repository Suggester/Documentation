### Changelog

### Suggester v4.7.2 (January 31st, 2021)
- The `ping` command has been redesigned to show more information and not error when the bot is starting up
- The `mark` command should no longer output an error if you don't specify a status in the command and select a reaction to choose one
- Voting totals (upvotes/downvotes) should be more accurate now
- **@everyone** and **@here** mentions for the `feedping` and `reviewping` elements now resolve correctly and ping intended users


### Suggester v4.7.1 (January 6th, 2021)
- We now support importing suggestions from the `Gaius Cicereius#3705` bot
- You can now enable/disable comment timestamps on the suggestion embeds using `cfg commenttime [on/off/toggle]` 

### Suggester v4.7 (January 4th, 2021)
- This release brings a new major feature to the bot: a Trello integration! We have a new documentation page for it, which can be found [here](/trello/intro.md), and you can also use `config help trello` to find more examples
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

### Suggester v4.6.1 (December 14th, 2020)
- Added a comment editing feature for server staff! You can now use `editcomment [comment ID] [new content]` to modify comments either posted by you or posted anonymously
- Fixed a bug where suggestions couldn't be deleted if their review channel had been deleted
- Added the "Read Message History" permission to some commands where the bot adds reactions
- Re-implemented and improved a legume-themed easter egg from a long time ago.. (we did it! 🎉)


### Suggester v4.6 (November 20th, 2020)
- The ability to edit suggestions has been added! Users can now edit suggestions they’ve submitted, and server admins/staff can edit any suggestion (the footer will show if the suggestion was edited by a staff member). A user editing their own approved suggestion in the review mode will send the edit for review
- Added a `shortinfo` command for when you want to show info about a suggestion in a concise manner without any internal information like the staff member who took action on it
- Added an implemented suggestion role (`cfg implementedrole`), so users who get their suggestions marked as Implemented can receive a role
- Added a configuration element to control auto-following server-wide (`cfg autofollow`) which is enabled by default
- The `top` command is now numbered 
- Server staff/admins are now exempted from the configured suggestion cooldown
- The character limit on suggestions has been raised to 1900 characters (previously 1024)
- The comment limit is now 15 comments per suggestion

🎉 **5000 Servers!!**

Thanks for helping Suggester reach 5000 Servers! To celebrate, we'll be giving out 10 VoteBoat votes to 5 winners in a giveaway on our [Support Server](https://discord.gg/G5pEdUp)! 

🍔 **Reddit**

Suggester is now present on Reddit! Join us at https://www.reddit.com/r/Suggester/ 

### Suggester v4.5.1 (October 21st, 2020)

This release primarily contains performance improvements for servers with a large number of approved suggestions/members who vote on suggestions:
- The `top` & `down` commands now use cached votes, which should considerably improve the time those commands take
- Changed notifications so that logging occurs first, which should reduce lag when a suggestion has a lot of followers
- Fixed a small issue with the `delete` command not working when the suggestion channel was changed
 

### Suggester v4.5 (October 17th, 2020)
It’s been a while since we released an update, but we’ve finally got some new stuff for you!

__New Features & Improvements__
- The `cleancommands` config element now applies to more commands. This was mainly applied to commands that are used frequently or where the response is mostly just to let you know the command succeeded. Both the command message and the bot response are deleted after 7.5 seconds.
- We’ve added a new suggestion cooldown (`config cooldown`) config element! After submitting a suggestion, users must wait the configured duration before submitting another. Server staff members can waive this cooldown using the `exempt` command.
- The `dupe` command has been added so that you can deny a suggestion as a duplicate of another. Usage is `dupe 1 2` (1 being the duplicate suggestion and 2 being the original)
- Removed the “You already have a suggestion awaiting review” message due to overall negative feedback
- `prefix` is now its own separate command
- 👻 

__Bugfixes__
- Fixed handling of the commands channel for servers who had one set before the 4.4 release
- System messages are no longer accepted for inchannelsuggestions
- Reactions are now removed from the review message when using massapprove/deny
- Other minor things


### Suggester v4.4 (September 18th, 2020)

- You can now __follow__ suggestions to be notified when they are updated. This works just like notifications sent to the suggester, but you can get them for suggestions you didn't submit. You can follow suggestions using the `follow` command and by upvoting any suggestion!
- Users can now be blocked from using the bot for a period of time using `block [user] [time]`
- You can now set multiple commands channels using `config commands add #channel`
- The `top` command now accepts a time argument, which filters the results for suggestions submitted only within the specified time
- The `down` command has been created, so now you can see a list of which suggestions your members don't like (this accepts a time argument too!)
- Attachments are now stored in a manner that allows `cleancommands` to work without the image not resolving 
- If you change the suggestions channel you should still be able to interact with suggestions that are in the old channel
- There is no longer a redundant reply message when you react to approve/deny
- The `github` command shows the link to Suggester's GitHub repository
 
We also added a new **large server** system. If your server has a large (as in several thousands) number of members or high volume of suggestions and would benefit from features like an increased `top` command view and reduced cooldowns for server staff members, contact our [Support Team](https://discord.gg/G5pEdUp) and we'll work from there.
 
