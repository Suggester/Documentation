# Configuration Element: Allowed Roles

### Description
Suggester bases its permission system the same as Discord, by using different roles. Allowed roles will define what roles users must have to be able to send suggestions via the `.suggest` command.\
If no roles are configured, all users can submit suggestions.

### Usage
Set up allowed roles using `.config allowed add/remove/list [role]`

### Aliases
`allowedrole`, `suggestrole`

### Accepted Inputs
Any role name, id or @mention

?> Users will only need **one** of those roles to be able to submit suggestions.
