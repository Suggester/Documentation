# Configuration Element: Voting Roles

### Description
Suggester bases its permission system the same as Discord, by using different roles. Voting Roles are allowed to vote on suggestions in the approved suggestion feed.\
If no roles are configured, all users can vote on suggestions.

### Usage
Set up voting roles using `.config voting add/remove/list [role]`

### Aliases
`voterole`, `voteroles`, `votingroles` and `votingroles` 

### Accepted Inputs
Any role name, id or @mention

?> If someone with none of the voting roles tries to vote on a suggestion, Suggester will instantly remove their reaction.
