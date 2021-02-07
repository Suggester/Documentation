# Command: deny
---
### Description
Use this command to deny a suggestion, sending it to the configured [denied suggestions channel](/config/denied.md) 

?> This command is only available when the mode is set to **review**

### Usage
Use `.deny [suggestion ID] (reason)` in any channel the bot can read & send messages in

### Arguments
`suggestion ID`: The ID of the suggestion you'd like to deny\
`reason`: The reason for the denial (optional)

### Aliases
`reject`, `refuse` and `no`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role
