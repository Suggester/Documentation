# Configuration Element: Voting Roles

### What is it for?
Suggester bases its permission system the same as Discord, by using different roles. Voting Roles are allowed to vote on suggestions in the approved suggestion feed.\
If no roles are configured, all users can vote on suggestions.

### Usage
Set up voting roles using `.config voting add/remove/list [role]`

### Accepted Imputs
Any role name, ID or @mention

📝 **Note:** If users try to vote on a suggestion while they don't have any voting role, the bot will instantly remove their reaction! 
