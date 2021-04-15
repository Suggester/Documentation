# Configuration Element: Implemented Suggestion Role

### What is it for?
This setting defines a role that will be given to members when one of their suggestions is marked as Implemented using the [`mark`](staff/mark.md) command

### Usage
Set up the given role using `.config implementedrole [role]`, setting `none` as the role will reset the current configuration meaning no roles will be given. 

### Accepted Imputs
Any role name, ID or @mention

?> Integration roles cannot be set as the implemented-role, this includes bots’ roles, boosting, Twitch subs, YouTube subs and the **@everyone** role.
