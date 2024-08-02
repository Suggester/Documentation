# Command: deny
---
### Description
Use this command to deny a suggestion, sending it to the configured [denied suggestions channel](/config/denied.md) 

?> This command is only available when the mode is set to **review**

### Usage
Use `.deny [suggestion id] (reason)` in any channel the bot can read and send messages in.

### Arguments
`suggestion id`: The id of the suggestion you want to deny\
`reason`: The reason for the denial (optional)

### Aliases
`reject`, `refuse` and `no`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role.
