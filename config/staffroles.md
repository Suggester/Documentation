# Configuration Element: Staff Roles

### Description
Suggester bases its permission system the same as Discord, by using different roles. Staff roles define what roles will be able to use staff-only commands (such as `.approve`). Any role configured as staff will automatically receive all staff permissions, and thus the ability to manage server suggestions.

### Usage
Set up a staff role using `.config staff add/remove/list [role]`

### Aliases
`staffroles`, `staffrole` and `reviewrole`

### Accepted Inputs
Any role name, ID or @mention

!> Adding the **@everyone** role as a staff role will give **all members of your server** enhanced permissions on the bot!
