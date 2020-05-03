# Mark
---
### Description
This command is used to change the status of a suggestion.
### Required Arguments
`suggestion ID` - The ID of the suggestion you want to change it's status.

`status` - The status you want to use.

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
