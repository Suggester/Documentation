# Configuration Element: Admin Roles

### Description
Suggester bases its permission system the same as Discord, by using different roles. Admin roles define what roles will be able to use admin-only commands (such as `.config` for example). Any role configured as admin will automatically receive all staff permissions, plus the ability to configure server settings.

### Usage
Set up an admin role using `.config admin add/remove/list [role]`

### Aliases 
`adminrole` and `adminroles`

### Accepted Inputs
Any role name, id or @mention

!> Adding the @everyone role to the configuration will give **all members of your server** elevated permissions on the bot!