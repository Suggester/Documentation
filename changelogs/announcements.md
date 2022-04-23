# Announcements

### What's Next for Suggester (October 13rd, 2021)
On July 29th 2021, Discord announced that access to [message content will become a privileged intent](https://support-dev.discord.com/hc/articles/4404772028055) for developers maintaining verified bots, starting in April of 2022.\
**Update**: The deadline has been postponed to September 1st, 2022.

**Today**\
In the current state, all but one of Suggester's commands rely on reading user messages to check for the prefix and then parse command data from the content. Following this annnouncement, **we are starting a migration to interactions**, which includes:
- Moving from prefixed to slash commands  
- Replacing reactions with buttons
- Improving the user experience using various message components and context menus

**Release**\
We hope to see these changes before the restrictions enter into effect. Unfortunately, we do not have an ETA to share just yet. We will be rebuilding Suggester from the ground up, so it will take some time before the update is ready.

**Staying Updated & Participating**\
In the meantime, we've created a new selfrole that you can get in the [support server](https://suggester.js.org/support) which we'll regularly ping for polls and other things related to the rewrite. Some changes might have some impact on how you use the bot, so it is important for us to hear your thoughts about what we're doing; and how we're doing it.


### Custom Instances & Donations (August 27th, 2021)
We're excited to announce our new Custom Instance program and Ko-fi donation page, https://ko-fi.com/suggester! For users who donate at least $5/month, we will host an instance of the bot with your own custom branding!

You can subscribe to one of the three tiers by going to http://ko-fi.com/suggester/tiers. After subscribing, contact us in our support server and we'll get it setup for you!

I want to support Suggester, but don't want to make a recurring purchase! On the Ko-fi page, there is a one-time donation option! We don't offer custom instance hosting for one-time donations, but you do get to permanently rep a fancy purple Donator role on the support server!

More info can be found [here](/supporting/info.md)

### Status Page (August 25th, 2021)
Not a downtime for once! We now have a status page for real time downtimes and maintenances which you can find at https://suggester.js.org/status 
It comes with a built-in subscription system where you can get updates from us sent directly to your email, simply by clicking the blue button at the top. We'll continue to announce outages in the support server for the time being.

A few past incidents were backfilled so it doesn't look too empty when we announce it but don't fret, Suggester is working :D

### An Update on the Latest Extended Downtime (August 23rd, 2021)
On August 14th, some unauthorized users obtained access to Suggester's database, allowing them to see and remove any data we stored. This caused issues when trying to access it, such as when interacting with old suggestions or setting up a server.

At first we thought this was a genuine issue with the database and thus kept the bot online so people could at least still send suggestions in their favorite servers, if said servers went through some configuration again.

But on August 15, the entirety of our collected data was removed, preventing Suggester from working. After discovering the whole issue, we've decided to bring all public instances of Suggester offline, as an unplanned maintenance due to a major service disruption.

As per Discord's Developer Policy and Legal Agreement, we must inform our users if any unauthorized users or group of users had access to any data we store, and sadly here we are. We believe the data accessed consisted of server setups, suggestion content and user settings. What we store can be found [here](/legal.md).

We have no reason to believe the compromised data was seen or shared by unauthorized third parties before being completely erased.

Suggester will be coming back online in the next few hours with our latest backup, from July 10th. As such, **any data added, removed or edited between that date and the beginning of this downtime will not be available.**

We are still actively investigating how this happened, but in the meantime the bot will be running on a new, much more secure server. We will be doing everything in our power to stop this from happening again.

As a side note, we'll be adding support for Suggester, Suggester 2 and Suggester Canary to the `.import` command, as well as a temporarily raised importing limit so you can hopefully get some of the data back.

On behalf of the entire Suggester team, we are extremely sorry for everything that has happened.

### An Update on Recent Infrastructure Issues (June 25th, 2021)
We are aware Suggester has had several performance issues in the last few weeks and we are deeply sorry for that. We believe those issues are related to the rather quick growth of Suggester, as its server count was **multiplied by more than 5** in the last year (victim of its success!). 

Past 2,500 guilds, a process that goes by the name of *sharding* goes from recommended to required (for those of you who don't know what that is, it's basically splitting your bot into multiple connections to the Discord API instead of a single one). While deploying new shards is done automatically and thus very simple, supporting an increasing number of these impacts performance metrics such as memory usage and overall latency. That is why Suggester has been slower than usual recently.

However, this isn't the end of the road. Our development team is currently made of **2 awesome person** that take these issues very seriously and they are working on solving them. Due to the nature of the problem, it will take some time to completely get back to normal performances.

As some testers might have already noticed, the canary bot is undergoing caching-related changes that may improve performances. Though as the name implies, it isn't production ready just yet.

### Suggester Rebranding (May 13th, 2021)
Discord has [rebranded](https://dis.gd/ournewlook), changing their old blurple color (#7289DA) to a new brighter blue (#5865F2). Since Suggester's profile picture and default color scheme used the OG Blurple color, we're rebranding our icons and assets as well! You'll notice a brand new Suggester icon, as well as a new default color for suggestion embeds and some emojis used by the bot.

### 2nd Birthday (April 7th, 2021)
Happy Birthday!! Suggester turned 2 on April 7th! That's pretty cool 😱

### Reddit (November 20th, 2020)
Suggester is now present on Reddit! Join us at https://www.reddit.com/r/Suggester/

### Suggester 2 joins the family! (May 8th, 2020)
We’ve been getting this request for a while, especially more recently: Having multiple suggestion channels/multiple instances. We decided to make this happen, and now Suggester 2 exists! If you operate a server with multiple suggestion channels, you can use Suggester for one and Suggester 2 for the other!

They are the same bot in almost every way, except they run on different databases (configs/suggestions do not sync between them) and the default prefix for Suggester 2 is `,`

### New Voting Sytem (March 23rd, 2020)
You may have noticed things changing with our voting system over the past few days... and we're happy to announce that the newest version of **VoteBoat** is finally ready!

- Added support for all bot lists that have a voting feature
- Added streaks. Voting five times in a row (either per 12-hour period or per day depending on the list) will get you one extra vote per 5 day streak!
- top.gg votes are worth 2 on weekends, so you get 2 votes counted here for weekend votes as well!
- Bots on Discord reviews are worth 3 votes, once you submit a review [here](https://bots.ondiscord.xyz/bots/564426594144354315/review), use `v!checkreview` to get your extra votes!
- Added new rewards for voting (and changed the cost of old rewards, since now you can get a lot more votes daily)
- Made voting reminders arrive on time  
- Updated `#voting-info` to look much cooler 😎 
- Made VoteBoat open source (https://github.com/Suggester/VoteBoat)

Your old vote counts have stuck around as well, they're included in your total.

### Important Announcement (January 28th, 2020)
On December 11th 2019, Suggester began to encounter issues. These were due to the bot using too much of the memory that it was allotted. Over four thousand suggestions had been submitted, and hundreds of servers configured. With the bot’s database (Enmap) based in the application memory, once it used too much memory we were in trouble. Looking at the database documentation, there was a way to reduce memory usage, so we implemented that in order to keep the bot stable.

And this did work, but unfortunately not for long. On December 12th - one day later -, the memory began to hit critical levels again. This time, there was no easy fix to reduce memory usage. We decided to move hosts to hopefully solve this issue, but it took some time to get the bot operational from the new host. Every so often, issues popped up like the bot not staying online, or sometimes suggestions and server configurations getting randomly lost. Overall, the move to the new host wasn’t going too well. On December 21st, the bot went down again. As usual, we went to boot it back up - but when we accessed the code we realized that everything was gone. Our database and code were nowhere to be found. This is when we began fully rewriting the bot to a new database, and locked it indefinitely. Now, after a little more than a month, we’re finally ready to release the new version of the bot and get Suggester operational again. We’ve overhauled every file, switching our database to an externally hosted version on MongoDB to ensure reliability. We have also decided to **make the bot open source**, and you can find the code at https://github.com/Suggester/Suggester. The bot is now open to community contributions - so if you want to see something added to Suggester, submit a pull request! We have the nice, shiny **Contributor** role for anyone who takes the time to make a major contribution to the bot.

Thanks to our Canary testers who helped test this new version of the bot, and everyone who voted for Suggester even during the issues. We greatly appreciate it ❤️

All of the database data from the beginning of these issues (December 12th, 2019) was ported over to our new database, so most existing suggestions (4000+ of them) should still be there, as well as old server configurations. Thanks for sticking with us while we fixed these issues, happy suggesting! 

*- The Suggester Dev Team*
