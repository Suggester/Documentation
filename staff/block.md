# Command: block
---
### Description
Use this command to prevent specific people from using the bot in the server

### Usage
Use `.block [user] (duration)` in any channel the bot can read and send messages in.

### Arguments
`user`: The user you want to block

?> You can use usernames, IDs and mentions.


`duration`: The duration you want to block the user for (optional)

### Duration & Examples
See the table below for more information on how to format durations


| Name     | Shortcut |
|:--------:|:--------:|
| seconds  | s        |
| minutes  | m        |
| hours    | h        |
| days     | d        |
| weeks    | w        |

### Examples
![Blocking](../images/blocking.png)

### Alias
`disallow`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role.

?> If you want to block entire roles from using the bot on your server, you might want to configure [Blocked Roles](/config/blockedroles.md)!
