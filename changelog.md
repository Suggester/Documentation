# Changelog
### Suggester v4.6.1 (December 14th, 2020)
- Added a comment editing feature for server staff! You can now use `editcomment [comment ID] [new content]` to modify comments either posted by you or posted anonymously
- Fixed a bug where suggestions couldn't be deleted if their review channel had been deleted
- Added the "Read Message History" permission to some commands where the bot adds reactions
- Re-implemented and improved a legume-themed eastern egg from a long time ago.. (we did it! 🎉)


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
 
