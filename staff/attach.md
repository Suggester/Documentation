# Command: attach
---
### Description
Use this command to attach an image to a suggestion either pending review or already approved 

### Usage
Use `.attach [suggestion id] [attachment]` in any channel the bot can read and send messages in.

### Arguments
`suggestion id`: The id of the suggestion you want to attach an image to\
`attachment`: The image to attach, we currently support `.png`, `.jpg`, `.jpeg` and `.gif` files. To provide an attachment, you can either use a link (like imgur.com) or directly attach the file to your message ([How?](https://support.discord.com/hc/en-us/articles/211866427))

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role.


!> ⚠ **Important Note:** To maintain images even after the original command has been deleted (for example when `cleancommands` is enabled), we rehost attached files in a private channel only a few people have access to, see our [Privacy Policy](/legal.md) for more information.
