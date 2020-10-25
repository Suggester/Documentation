# Configuration Element: Staff Roles

### What is it for?
Suggester bases its permission system the same as Discord, by using different roles. Staff roles define what roles will be able to use staff-only commands (such as `.approve` for example)\
Any role configured as staff will automatically receive all staff permissions, and thus the ability to manage server suggestions.

### Usage
Set up a staff role using `.config staff add/remove/list [role]`

### Accepted Imputs
Any role name, ID or @mention

⚠ **Warning!** Adding the `@everyone` role to the configuration will give **all members of your server** enhanced permissions on the bot!
