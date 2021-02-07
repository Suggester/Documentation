# Beginner's Guide: Suggester Basics
---
Have you ever wanted a discord bot allowing you to manage suggestions as well as giving away free cookies? Well, Suggester only allows the former (good news, I guess?).. Okay, let's begin. 
It might sounds a bit complicated at first, but don't fret, we'll dive into it below.

First, you need to add Suggester to your server, you can do so with [this link](https://discord.com/oauth2/authorize?client_id=564426594144354315&scope=bot&permissions=805694544) (you'll need the **Manage Server** permission on the server you'd like to add the bot to). Suggester needs all listed permissions to function correctly, if any of these permissions are omitted, some functions may not work.

   ![Invite the bot](https://cdn.discordapp.com/attachments/769650556502409226/769650566858539039/unknown.png)

When you're done filling the captcha, go back to your server. Suggester should've sent a handy tutorial with some information about configuration, what a good introduction to what's next! 

![tutorial](https://cdn.discordapp.com/attachments/769650556502409226/769651554877702144/unknown.png)

Suggester uses a modern configuration system which allows admins to customize its behavior in each server. That being said, you now need to setup the bot in your server. 
There's two different ways to do that, the first one doesn't require anything but the usage of a command: send `.autosetup` in any channel the bot can read & send messages in, then let the magic happen! More information about automatic setup can be found [here](admin/autosetup.md).\
If you wish to do it yourself, you can use the [`.setup`](admin/setup.md) command to start an interactive guide! Simply respond to each prompt with a correct argument listed under the "Inputs" field of the setup embed.

![inputs](https://cdn.discordapp.com/attachments/769650556502409226/769653509711855646/unknown.png)

And you're done, you & your members can now start suggesting using the `.suggest` command in your server! If you wish to configure more settings like custom reactions, notifications and more, check out the [`.config`](config/configuration.md) command!


?> If you need any help configuring the bot, feel free to join our [Support Server](https://discord.gg/G5pEdUp) to receive assistance!
