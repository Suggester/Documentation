# Suggestion Handling Modes
Suggester currently offers **two different** modes for handling suggestions in your server. We have seen a lot of questions about how they work, so we'll dive into it below. As surprising as it might sound, this guide will be divided into two parts, one for each mode.

### Autoapprove
This mode is very simple and does not require any additional configuration elements! Any suggestion sent in your server will be automatically approved, skipping the review phase and sending it to your configured [approved suggestions channel](/config/suggestions). If later on, you need to remove these suggestions for whatever reason, you can do so by using the `.delete` command which will remove the suggestion embed and send it to the configured [denied suggestions channel](/config/denied), if set.

However, if you wish to tell your members you like this suggestion, you can set a status using the `.mark` command. You can find a list of statuses [here](/staff/mark)!

---
### Review
This one is a bit more complex as it relies on an extra configuration element, the [review channel](/config/review). When this mode is set, any suggestion from your members will be sent to your review channel where the server staff can decide whether it should be approved or not. It is useful for public servers where suggestions aren't necessarily good ideas. Yes, we tried to get our **#kitchen-sinks** channel, but it didn't live past the review phase. Sad trombone.

You can deny a suggestion using `.deny` and approve it using the `.approve` command. Make sure to check the general documentation to learn more about the managing commands Suggester currently provides and their syntaxes.


?> If you have any idea for a potential new mode, make sure to suggest it in our [support server](https://suggester.js.org/support)!

