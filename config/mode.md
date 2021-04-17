# Configuration Element: Suggestion Handling Mode

### Description
This setting defines how suggestions will be handled in your server, there are currently **two** available modes:
- **Review:** suggestions are held for manual review by staff (requires usage of managing commands + 
- **Autoapprove:** 

| Mode         | Description                                                                 | Additional Requirements                |
|:------------:|:---------------------------------------------------------------------------:|:------------------------------------------:|
| Review       | Suggestions are held for manual review                                      | [review channel](/config/review.md) and usage of the managing commands |
| Autoapprove  | Suggestions are automatically approved and sent in the suggestions feed     |                                            |


### Usage
Set up the mode using `.config mode review/autoapprove`

### Accepted Inputs
Any channel name, ID or #mention

?> If you wish to change the mode from `review` to `autoapprove`, you'll have to clear all pending suggestions by either approving or denying them. You can use the [`.listqueue`](/staff/listqueue.md) command to list all pending suggestions.
