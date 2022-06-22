# Known Issues
You can find below a list of issues we are aware of, alongside potential workarounds or more detailled information about the issue. This list was last updated on June 22nd.

### Reaction-related features don't work consistently
We are aware of certain features involving message reactions (like vote counters) not working at certain times. We believe the issue to be related to the fact that reactions aren't meant to be used as UI elements like buttons, as they are inconsistently sent to bots. If you encounter an issue involving reactions, it might fix itself after a while! If the issue is consistent, feel free to contact us in our [support server](https://suggester.js.org/support).

We plan to fix this in the next major version, by switching to message components throughout the bot.

### A suggestion I do not have access to despite being admin prevents me from changing the mode
This happens when the review message of a suggestion or the channel it was posted in is deleted when the suggestion is still pending. We recommend using managing commands **before** taking destructive actions such as deleting a channel.

If you are in this situation, reach out to our support team with some context and relevant suggesttion ids. 
