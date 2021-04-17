# Beginner's Guide: Suggester Basics
---
Have you ever wanted a discord bot allowing you to manage suggestions as well as giving away free cookies? Well, Suggester only allows the former (good news, I guess?).. Okay, let's begin. 
It might sound a bit complicated at first, but don't fret, we'll dive into it below.

First, you need to add Suggester to your server, you can do so with [this link](https://suggester.js.org/invite) (note that you'll need the **Manage Server** permission in the server you want to add the bot to). Suggester needs all listed permissions to function correctly, if any of these permissions are omitted, some functions may not work.

![Invite Suggester to your server](/images/invite.png) 

When you're done filling the captcha, go back to your server. Suggester should've sent a handy tutorial with some information about configuration, what a good introduction to what's next! 

![Suggester Tutorial](/images/tutorial.png)

Suggester uses a modern configuration system which allows admins to customize its behavior in each server. That being said, you now need to setup the bot in your server. 
There's two different ways to do that, the first one doesn't require anything but the usage of a command: send `.autosetup` in any channel the bot can read & send messages in, then let the magic happen! More information about automatic setup can be found [here](admin/autosetup.md).

If you wish to do it yourself, you can use the [setup](admin/setup.md) command to start an interactive guide! Simply respond to each prompt with a correct argument listed under the "Inputs" field of the setup embed.

![Interactive Setup](/images/setup.png)

And you're done! Members of your server can now start suggesting using the `.suggest` command! If you wish to configure more settings like custom reactions, notifications and more, check out the [config](/config/configuration.md) command!


?> If you need any help configuring the bot, feel free to join our [Support Server](https://suggester.js.org/support) to receive assistance!
