# Translating Suggester: Everything You Need To Know

Hey welcome! Thanks for your interest in translating Suggester, it means a lot! Before starting, let me explain how it works. 
We use the `i18n#1614` bot to handle translations, which means you will have to make sure your DMs aren't closed on the [support server](https://discord.gg/G5pEdUp) before starting. 

When you're done verifying, run the `>start` command in [`#translator-chat`](https://canary.discord.com/channels/566002482166104066/705524292690903060). The bot will then either start the process if you only have one authorized locale, or ask you to pick a locale code from your authorized ones

?> A **locale code** is a short string, usually composed of a few letters, which represents your language. For example, the locale code of the French language is `fr`, English's is `en`, etc.. 

### Dynamic Process Embed Fields

You might be wondering what are all those fields, so I'll explain below.


- The first field, named "**English String**", shows the original string you have to translate in your language, easy! 

- A few pixels below, you can see the "**Raw Content**" field, which basically shows the content with no magic used (no markdown no nothing). It is used to show how to add markdown and hyperlinks to the string.

- Another few pixels and you'll meet the "**Context**" field, it adds more details to each string to facilitate translation, especially for languages using gendered words or different grammatical syntaxes.

- Finally, the "**Parameters**" field lists, if any, all placeholders present in the string to translate. 

You can also find the name of the string you're currently translating on the embed's footer. In the below example, `CFG_COOLDOWN_SET` is the string name. 

![Translation Embed Fields](https://cdn.discordapp.com/attachments/769650556502409226/769980267124490270/unknown.png)



### The DOs and DONTs when translating

We currently don't support command names and arguments in other languages, meaning that you **must not** translate them. For example, `approve` will remain in english, same goes for command arguments (eg `on`, `off`, `toggle`, `list`, `add`, `remove`...). Words in `{{placeholders}}` represent real data and should also be kept in english.
However, syntax guiding (see example below) must be translated

![Syntax Guiding](https://cdn.discordapp.com/attachments/769650556502409226/769988849430298624/unknown.png)

Last but not least, don't forget to keep the [markdown](https://support.discord.com/hc/en-us/articles/210298617) when you translate a string (bold, italic, codeblocks etc..).

### Details

You have 5 minutes to translate a string, then 2 minutes to make sure it is correct and confirm it by clicking on the ✅ reaction. If you made a typo or want to retranslate it, click on the ❌! 

?> If you ever make a mistake after the string has been confirmed, don't worry! You can easily fix it, using the `>mt` command in `#translator-chat`.

?> **Syntax:** `>mt [locale code] [string name] [new translation]` 

As a thank you, every translator will get the "Translator" acknowledgement on the `.verify` command, as well as the ability to choose a custom one once they've translated a significant part the language.


Thanks for reading and good luck translating!

![ty](https://media4.giphy.com/media/elgNhgAyoH3vkfAACc/giphy.gif)
