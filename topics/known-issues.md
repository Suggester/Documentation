# Known Issues
You can find below a list of issues we are aware of, alongside potential workarounds or more detailled information about the issue. This list was last updated on April 12th, 2024. If you'd like to contact us, feel free to join the [support server](https://suggester.js.org/support).

### Attachments not displaying properly
We're aware of issues with images not resolving on suggestions.

### Reaction-related features don't work consistently
We are aware of certain features involving message reactions (like vote counters) not working at certain times. We believe the issue to be related to the fact that reactions aren't meant to be used as UI elements like buttons, as they are inconsistently sent to bots. If you encounter an issue involving reactions, it might fix itself after a while!

We plan to fix this in the next major version, by switching to message components throughout the bot.

### A suggestion I do not have access to despite being admin prevents me from changing the mode
This happens when the review message of a suggestion or the channel it was posted in is deleted when the suggestion is still pending. We recommend using managing commands **before** taking destructive actions such as deleting a channel.

If you are in this situation, reach out to our support team with some context and relevant suggestion ids.


