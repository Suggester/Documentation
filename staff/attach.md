# Command: attach
---
### Description
Use this command to attach an image to a suggestion either pending review or already approved 

### Usage
Use `.attach [suggestion id] [attachment]` in any channel the bot can read and send messages in.

### Arguments
`suggestion id`: The id of the suggestion you want to attach an image to\
`attachment`: The image to attach, as a `.png`, `.jpg`, `.jpeg` or `.gif` file. You can either use a direct link or [directly attach the file](https://support.discord.com/hc/en-us/articles/211866427) to your message.

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role.


!> ⚠ **Important Note:** To maintain images even after the original command has been deleted, we re-upload attachments in a private channel only Suggester Staff have access to, see our [privacy policy](/legal/privacy.md) for more information.