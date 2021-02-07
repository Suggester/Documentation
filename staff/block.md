# Command: block
---
### Description
Use this command to prevent specific people from using the bot in the server

### Usage
Use `.block [user] (duration)` in any channel the bot can read & send messages in

### Arguments
`user`: The user you want to block, you can use both IDs and mentions\
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

> **Examples**\
> Using `.block @poggers 2h no spam!`will block **@poggers** for 2 hours with reason "no spam!"\
> Using `.block @poggers 6d hahayes` will block **@poggers** for 6 days with reason "hahayes"

### Alias
`disallow`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role

?> If you want to block entire roles from using the bot on your server, you might want to configure [Blocked Roles](/config/blockedroles.md)!
