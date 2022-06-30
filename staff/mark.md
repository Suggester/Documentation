# Command: mark
---
### Description
Use this command to edit a suggestion's status.

### Usage
Use `.mark [suggestion ID] (status) (comment)`

### Arguments

`suggestion ID`: The ID of the suggestion you want to modify the status of

`status`: The new status you want to set, use the table below to find all available statuses (If no status is provided, an interactive menu will be shown to pick one)

| Argument              |                Meaning                |                 Context Examples                                                                         |
|-----------------------|:-------------------------------------:|-------------------------------------------------------------------|
| `default`, `none`, `reset`     | Resets status to default (none shown) |                                                                                                          |
| `no`, `not`                  | Not Happening                         | Used to let users know the suggestion will not be implemented                                            |
| `working`, `progress`, `inprogress` | In Progress                           | Useful to leak upcoming stuff 👀                                                                        |
| `implemented`, `done` | Implemented                           | Use this status when something has been implemented                                                      |
| `consideration`, `consider`, `considered`, `inconsideration`       | In Consideration                      | Handy status to let users know you're debating about the suggestion, but nothing official *yet*          |


`comment`: A comment to add to the suggestion (optional)

### Caveat
When marking a suggestion as Implemented, reactions will only be removed from the message if you have configured an [implemented suggestions channel](../config/implemented.md).

### Alias
`status`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role.
