# Editing a suggestion
Mistakes happen, when your grammar randomly decides to take a nap when suggesting something, you can now fix it using the shiny `.edit` command! 

### Users
Regular users can only edit their own approved suggestion(s). If the mode is set to [review]/config/mode.md), any edit will require approval by a staff member to be updated in the sugggestion feed. If the suggestion is edited by someone with staff or admin permissions, no approval is required.

### Staff & Admins
Users with staff or admin permissions can edit **any** suggestion, with no approval required. If the suggestion has been edited by a server staff member, it will be displayed along their username on the suggestion embed.

![edited by a server staff member](https://cdn.discordapp.com/attachments/769650556502409226/782613453437140992/unknown.png)

If the mode is set to [review]/config/mode.md), all editing requests from users with no elevated permissions will require approval to update the suggestion. To handle these editing requests, members with staff or admin permissions can use the [`approveedit`](/staff/approveedit.md) and [`denyedit`](/staff/denyedit.md) commands or simply click on the corresponding reactions on the message sent in the [review](config.review.md) channel.

![pending edit request](https://cdn.discordapp.com/attachments/769650556502409226/782617101940162560/unknown.png)

### Usage
Use `.edit [suggestion ID] (new content)` in any channel the bot can read and send messages in.

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
