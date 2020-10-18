# Configuration Element: Admin Roles

### What is it for?
Suggester bases its permission system the same as Discord, by using different roles. Admin roles define what roles will be able to use admin-only commands (such as `.config` for example)\
Any role configured as admin will automatically receive all staff permissions, plus the ability to configure server settings.


### Usage
Set up an admin role using `.config admin add/remove/list [role]`

### Accepted Imputs
Any role name, ID or @mention

⚠ **Warning!** Adding the everyone role to the configuration will give **all members of your server** enhanced permissions on the bot!
