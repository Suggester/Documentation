# Command: block
---
### Description
Use this command to prevent specific people from using the bot in the server

### Usage
Use `.block [user] (duration)` in any channel the bot can read and send messages in.

### Arguments
`user`: The user you want to block, you can use usernames, IDs and mentions.

`duration`: The duration you want to block the user for (optional, permanent if not provided)

### Duration & Examples
You can use "s" for seconds, "m" for minutes, "h" for hours and "d" for days.

### Examples
![An example usage of the blocking command](../images/blocking.png)

### Alias
`disallow`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role.

?> If you want to block entire roles from using the bot on your server, you might want to configure [Blocked Roles](/config/blockedroles.md)!
