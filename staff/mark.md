# Command: mark
---
### Description
Use this command to edit the displayed status of a suggestion.

### Usage
Use `.mark [suggestion id] [status] (comment)`

### Arguments

`suggestion id`: The id of the suggestion you want to modify the status

`status`: The new status you want to set, use the table below to find all available statuses:

| Argument              |                Meaning                |
|-----------------------|:-------------------------------------:|
| `none`, `reset`       | Resets status to default (none shown) |
| `no`                  | Not Happening                         |
| `working`, `progress` | In Progress                           |
| `implemented`, `done` | Implemented                           |
| `consider`            | In Consideration                      |


`comment`: A comment to add to the suggestion (optional)

### Caveat
When marking a suggestion as Implemented, reactions will only be removed from the message if you have configured an [implemented suggestions channel](../config/implemented.md).

### Alias
`status`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role.