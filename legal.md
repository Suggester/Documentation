# Privacy and Security Information
In order for the bot to function, we store some information about servers and users. Below you can find a list of what information we store and why it is stored.

## Data We Store
- User IDs: We store these to link suggestions to the user who suggested them, so that the bot can show the user who submitted the suggestion. Additionally, they are used to store a list of blocked users in each server and globally.
- Channel IDs: We store these so that the bot can know where to send various messages such as suggestion-awaiting-review messages, suggestion messages, denied suggestion messages, and log messages.
- Role IDs: We store these to allow server admins to configure roles that have certain permissions on the bot (staff, admin, blocked roles, etc.)
- Server IDs: We store these to keep server configurations and suggestions tied to their respective servers
- Webhook URLs: We store these to ensure logging through webhooks works - only one URL is stored which is the URL of the webhook created by the bot when logging is configured.
- Server Emotes: We store server emote names/IDs if a server configures an emote as a reaction emote in the suggestion feed
- Submitted Suggestions/Comments: We store message content submitted as suggestions and comments in order for the bot to have data about each suggestion
- Attachment URLs: We store URLs of files attached to suggestions in order to make the attaching feature possible.
- We log commands used and servers the bot is added to/removed from for analytical purposes.

## Why We Need & How We Use The Data
This data is used throughout the bot to make it work. Without storing the data above, it would not be possible for Suggester to function. The data we collect is used for the purposes stated above, and nothing else. We will never give out the information we store to unauthorized users.
 
## Security
All data and bot services are protected by authentication and access is limited to a small subset of users (developers, and (for some data) Suggester staff members). If you believe you have found a security issue in one of our systems, **do not** post in a public chat. DM a Developer (Brightness™#0001 or @Ben.#0002) with information and we will investigate.

## Concerns
If you have any concerns about the data we store or the functions of the bot, contact a member of the Suggester staff team or our Support bot that you can find in the [support server](https://discord.gg/G5pEdUp). 
We'll be more than happy to clear up any concerns you may have.
If you would like your data to be removed from our systems, please contact one of the developers listed above and we'll help you out from there.
