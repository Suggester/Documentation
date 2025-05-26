# Suggester Trello Integration
Introducing the **Suggester x Trello Integration**! You are now able to connect a Trello board to your server, and automatically organize suggestions based on actions you take on them directly on Discord using Suggester! Each action is customisable and will allow you to keep things organized pretty easily. You might be wondering a few things, so we'll dive into it below.

### What is Trello?
[Trello](https://trello.com) is a free collaboration software that helps users and companies organizing projects with the usage of modern management tools. You first create a board, add members to it and you can start dispatching different tasks!\
"Imagine a white board, filled with lists of sticky notes, with each note as a task for you and your team."

### How do I start?
First, you'll need to create a Trello account, you can do so by clicking [here](https://trello.com/signup). Once done, [create a board](https://trello.com/guide/create-a-board) and [add](https://help.trello.com/article/717-adding-people-to-a-board) `@suggester_bot` to it. Go back on Discord and run [`.config trello board [board link]`](/topics/trello/board.md) in a server where you have admin perms in to connect the board to your server.

If you later decide to not use Trello, you can type "none" as the board link in the above syntax to reset it.

### Event & Actions
You can configure Suggester to do certain actions when any of the following events occur:
- Someone creates a suggestion
- A suggestion is approved (available in review mode only)
- A suggestion is marked as Implemented
- A suggestion is marked as In Progress
- A suggestion is denied
- A suggestion is deleted

Actions that you can configure are:
- Moving a suggestion to a list
- Adding a [label](https://help.trello.com/article/797-adding-labels-to-cards) to a suggestion
- Removing a suggestion from the board
- Archiving a suggestion

### Usage & Examples
To add a new action to run when a certain event occurs, use the following syntax in any channel the bot can read and send messages in:

`.config trello actions [event] [action]`

#### Arguments
`[event]` can be "suggest", "approve", "implemented", "deny", "delete" or "working"\
`[action]` can be "list", "label", "delete, "archive" or "none" (to reset the assigned action)

#### Examples

| Description                                             | Link                                                                               |
|:-------------------------------------------------------:|:----------------------------------------------------------------------------------:|
| Add approved suggestions to a list                      | [Click](/topics/trello/approved-suggestions.md)                        |
| Archive deleted suggestions                             | [Travel your cursor around here, then hit](/topics/trello/deleted-suggestions.md)  |
| Remove deleted suggestions from the Board               | [Place your pointer then push it here](/topics/trello/deleted-suggestions.md)      |
| Give a label to suggestions marked as Implemented       | [Pop your mouse while hovering this](/topics/trello/marked-as-implemented.md)      |
| Add new suggestions to a list                           | [Deliver a quick click on this link](/topics/trello/new-suggestion.md)             |

### That's all folks
If you need help, want to report a bug, have any questions or feedback, feel free to join our [support server](https://suggester.js.org/support).


> Suggester is not affiliated with Trello.