# Mark
---
### Description
This command is used to change the status of a suggestion.
### Required Arguments

`suggestionId` - The ID of the suggestion.

`status` - The status you want to set.

| Argument              |                Meaning                |
|-----------------------|:-------------------------------------:|
| `default`, `none`     | Resets status to default (none shown) |
| `no`                  | Not Happening                         |
| `working`, `progress` | In Progress                           |
| `implemented`, `done` | Implemented                           |

### Optional Arguments
`comment` - A comment you want to add to the suggestion

### Usage
```
.mark <suggestionId> <status> (comment)
```
### Aliases
`status`
### Permission Required
The user must have **Manage Server** or a configured staff role.
