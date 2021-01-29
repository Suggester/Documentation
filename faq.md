# Suggester FAQ
You will find below a summary of questions we often see asked, if your question isn't answered here, join our [Support Server](https://discord.gg/G5pEdUp) and ask!

### Will kicking and adding Suggester back help in fixing my issue?
Most likely not, as settings stay stored even if the bot is kicked and re-added. If you're having an issue, contact our Support Team and we'll look into it further.

### Suggester isn't responding in my server, what can I do?
First, make sure you are using the correct prefix (you can check using `@Suggester#8366 prefix`). If you're using the right prefix, it might be a permission issue: Make sure Suggester has correct permissions, it needs at least **Read Messages**, **Send Messages** and **Embed Links** in the channel you're trying to use commands in

If none of the above solved your issue, let us know in our [Support Server](https://discord.gg/G5pEdUp)!

### How do I find a comment's ID?
Some commands will use a comment's ID as an argument. To find the ID of a comment, look at its field name, it will be displayed after the comment author's tag (if the comment is anonymous, it will be shown after ''Staff Comment'').
A comment's ID is formed by the ID of the suggestion its on followed by `_` and the number of total comments on this suggestion.\
In the example picture below, the comment ID is `12345_1`

![Comment ID Example Picture](https://cdn.discordapp.com/attachments/672037775154872323/769565201666146355/unknown.png)

### I found a bug, how do I report it?
If you want to report a bug, you'll need to be part of our [Canary Program](community-programs?id=🐛-hunting-bugs)

### How do I set a locale?

Suggester offers many different locales, so you can choose what language the bot will use when you'll use it! Locales can be configured on a per-user and per-server basis.

- To configure your User locale, use the `.locales` command to see the list of all available languages. Find the one you want, then use `.locale [name]` to set it!
- To configure your Server locale, use the [`.config locale`](/config/locale.md) command to see all available languages. Find the one you want, then use `.config locale [name]` to set it!

If your language isn't there and you want to translate it, take a look at our [Translation Program](community-programs.md)

### What is Suggester 2 & how can I invite it to my server?
Suggester 2 is identical to Suggester in almost every way! It allows you to manage two different suggestion setups with different settings in your server. Its default prefix is a comma (`,`) but you can indeed change it at any time by doing `@Suggester 2#6730 config prefix [new prefix]`

You can add it to your server with this [link](https://discord.com/oauth2/authorize?client_id=708299727166242866&scope=bot&permissions=805694544)

![Suggester 2 New Prefix](https://cdn.discordapp.com/attachments/672037775154872323/769566499807035422/unknown.png)




