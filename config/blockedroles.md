# Configuration Element: Blocked Roles

### What is it for?
Suggester bases its permission system the same as Discord, by using different roles. Blocked roles define what roles will be prevented from using the bot at all in the server\
If you want to block a specific user, use the [`.block`](staff/block.md) command.

### Usage
Set up blocked roles using `.config blocked add/remove/list [role]`

### Accepted Imputs
Any role name, ID or @mention

📝 **Note:** Staff/Admin users will still be able to use the bot, even if they have one or more blocked roles
