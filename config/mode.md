# Configuration Element: Suggestion Handling Mode

### What is it for?
This setting defines how suggestions will be handled in your server, there are currently **two** available modes:
- **Review:** suggestions are held for manual review by staff (requires usage of managing commands + a configured [review](configuration/review.md) channel)
- **Autoapprove:** suggestions are automatically approved and sent in the suggestion feed

### Usage
Set up the mode using `.config mode review/autoapprove`

### Accepted Imputs
Any channel name, ID or #mention

?> If you wish to change the mode from `review` to `autoapprove`, you'll have to clear all pending suggestions by either approving or denying them. You can use the [`.listqueue`](/staff/listqueue.md) command to list all pending suggestions.
