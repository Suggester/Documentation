# Editing a suggestion
Mistakes happen, when your grammar decides to randomly take a nap when suggesting something, you can now fix it using the shiny `.edit` command! 

### Users
Regular users can only edit their own approved suggestion(s). If the mode is set to [review](config/mode.md), any edit will require review by a staff member unless it is edited by someone with staff or admin permissions

### Staff & Admins
Users with staff or admin permissions can edit any suggestions, with no approval required. If the suggestion has been edited by a server staff member, it will be displayed along their username on the suggestion embed.

![edited by a server staff member](https://cdn.discordapp.com/attachments/769650556502409226/782613453437140992/unknown.png)

If the mode is set to [review](config/mode.md), all editing requests from users with no elevated permissions will require approval to update the suggestion. Staff and admin members can use the [`approveedit`](editing/approveedit.md) and [`denyedit`](editing/denyedit.md) commands, as well as clicking on the corresponding reactions on the message sent in the [review](config.review.md) channel to handle these edits.

![pending edit request](https://cdn.discordapp.com/attachments/769650556502409226/782617101940162560/unknown.png)

### Usage
Use `.edit [suggestion ID] (new content)` in any channel the bot can read & send messages in

### Arguments

`suggestion ID`: The ID of the suggestion you’d like to edit. If you don't have staff/admin perms, you can only edit your own suggestions\
`new content`: The edited version of the suggestion

!> Once you've edited a suggestion, you cannot restore its original content! 

### Permissions

| Permission                          | Editing all suggestions | Editing own suggestions |
|-------------------------------------|:-----------------------:|-------------------------|
| [Admin](/config/adminroles.md)      | ✓                       | ✓                       |
| [Staff](/config/staffroles.md)      | ✓                       | ✓                       |
| None                                | ⨉                       | ✓                      |
