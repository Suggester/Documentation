# Command: mark
---
### Description
Use this command to modify a suggestion's status

### Usage
Use `.mark [suggestion ID] [status] (comment)`

### Arguments

`suggestion ID`: The ID of the suggestion you'd like to modify the status.

`status`: The new status you want to set, use the table below to find all available statuses (If no status is provided, an interactive menu will be shown to choose one)

| Argument              |                Meaning                |                 Context Examples                                                                         |
|-----------------------|:-------------------------------------:|-------------------------------------------------------------------|
| `default`, `none`     | Resets status to default (none shown) |                                                                                                          |
| `no`                  | Not Happening                         | Used to let users know the suggestion will not be implemented                                            |
| `working`, `progress` | In Progress                           | Useful to leak upcoming stuff 👀                                                                        |
| `implemented`, `done` | Implemented                           | Use this status when something has been implemented                                                      |
| `consideration`       | In Consideration                      | Handy status to let users know you're debating about the suggestion, but nothing official *yet*          |


`comment`: A comment you want to add to the suggestion (optional)


### Alias
`status`

### User Permission
To execute this command, the user must have the **Manage Server** permission or a configured [staff](/config/staffroles.md) role
