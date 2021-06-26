# Announcements

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
