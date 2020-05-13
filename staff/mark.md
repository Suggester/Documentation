# Mark
---
### Description
This command is used to change the status of a suggestion.
### Required Arguments
`suggestion ID` - The ID of the suggestion you want to change the status of.

`status` - The new status you want to set on the suggestion.

| Argument              |                Meaning                |
|-----------------------|:-------------------------------------:|
| `default`, `none`     | Resets status to default (none shown) |
| `no`                  | Not Happening                         |
| `working`, `progress` | In Progress                           |
| `implemented`, `done` | Implemented                           |


### Usage
```
.mark [suggestion ID] [status]
```
### Aliases
`status`
### Permission Required
Any user with the **Manage Server** permission, a configured admin role or a configured staff role can use this command.
