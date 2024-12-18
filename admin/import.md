# Command: import
---
### Description
Import suggestions from regular users and [supported bots](admin/import.md?id=supported-bots) to manage them using Suggester. If you choose to import messages from a channel, Suggester will count any message as a suggestion, so make sure to remove any unwanted messages before processing. Messages can only be added to the database **once**, using the command again will not import the same suggestion twice.

### Usage
Use `.import` in a channel to import the last **30 messages** as suggestions. If you need to import more, you will have to delete the last 30 messages after they were imported. As such, we recommend creating a new channel when importing lots of suggestions from another bot.

!> If you need to import more suggestions at once, our [support team](https://suggester.js.org/support) can temporarily raise the limit to **100 messages**. Make sure to provide your [server id](https://dis.gd/findmyid) when contacting us about higher limits. 

### Permissions
To execute this command, the user must have the **Manage Server** permission or a configured [admin](/config/adminroles.md) role.

!> If it does not work, make sure Suggester has the **Read Message History** permission in the channel you're trying to import suggestion from.

### Supported Bots
Suggester supports importing suggestions from the following bots:

- ,Havoc#7078
- AXVin#4169
- Anchor#8635
- Carl-bot#1536
- Fast Bot.#2211
- Gaius Cicereius#3705 
- Juzo#2390
- Kashima#4514
- Suggestion#2670
- Suggestions#2602
- Suggestions#3153
- Suggestions#6994
- Ticks#3610
- UnbelievaBoat#1046
- UnbelievaBoat Premium#3539
- Zira#9472
