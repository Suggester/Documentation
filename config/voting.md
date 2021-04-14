# Configuration Element: Voting Roles

### What is it for?
Suggester bases its permission system the same as Discord, by using different roles. Voting Roles are allowed to vote on suggestions in the approved suggestion feed.\
If no roles are configured, all users can vote on suggestions.

### Usage
Set up voting roles using `.config voting add/remove/list [role]`

### Aliases
`voterole`, `voteroles`, `votingroles` and `votingroles` 

### Accepted Imputs
Any role name, ID or @mention

?> If someone with none of the voting roles tries to vote on a suggestion, Suggester will instantly remove their reaction.
