# Suggester Trello Integration
Our awesome developer's latest feature just got out of the oven, introducing the **Suggester Trello Integration**. You will be now be able to connect a Trello board to your server, and automatically organize suggestions based on actions you take on them directly on Discord using our bot! Each action is fully customisable and will allow you to keep things organized pretty easily\
You might be wondering a few things so we will dive into it below.

### What is Trello?
[Trello](https://trello.com) is a free collaboration software that helps users and companies organizing projects by the usage of modern management tools. You first create a board, add members to it and you can start dispatching different tasks!\
"Imagine a white board, filled with lists of sticky notes, with each note as a task for you and your team."

### How do I start?
First, you'll need to create a Trello account, you can do so by clicking [here](https://trello.com/signup). Once done, create a Trello board (if you don't know how, check this [guide](https://trello.com/guide/create-a-board)) and add `@suggester_bot` to it ([How?](https://help.trello.com/article/717-adding-people-to-a-board))
Back on Discord, let's setup Suggester: \
Run `.config trello board [board link]` in a server you have admin perms in to connect your board to your discord server, or click [here](/trello/board.md) for more info.

### Event & Actions
You can configure Suggester to do certain actions when any of the following events occur:
- Someone suggests something
- A suggestion is approved (review mode only)
- A suggestion is marked as Implemented
- A suggestion is marked as In Progress/Working
- A suggestion is denied
- A suggestion is deleted

Actions that you can configure are:
- Moving a suggestion to a list
- Giving a [label](https://help.trello.com/article/797-adding-labels-to-cards) to a suggestion
- Removing a suggestion from the board
- Archiving a suggestion

### Usage & Examples
To add a new action to run when a certain event occurs, send the following syntax in any channel the bot can read & send messages in:

`.config trello actions [event name] [action name]`
#### Arguments
`[event name]` can be `suggest`, `approve`, `implemented`, `deny`, `delete` or `working`\
`[action name]` can be `list`, `label`, `delete`, `archive` or `none` (to reset the assigned action)

#### Examples

| Description                                             | Link                                                                               |
|:-------------------------------------------------------:|:----------------------------------------------------------------------------------:|
| Add approved suggestions to a list                      | [Click Click Click](/trello/events/approved-suggestions.md)                        |
| Archive deleted suggestions                             | [Travel your cursor around here, then hit](/trello/events/deleted-suggestions.md)  |
| Remove deleted suggestions from the Board               | [Place your pointer then push it here](/trello/events/deleted-suggestions.md)      |
| Give a label to suggestions marked as Implemented       | [Pop your mouse while hovering this](/trello/events/marked-as-implemented.md)      |
| Add new suggestions to a list                           | [Deliver a quick click on this link](/trello/events/new-suggestion.md)             |

### That's all folks
This feature is fairly complex as we want to provide a lot of customizability for servers who use the Trello feature. If you need help, want to report a bug, have any questions or feedback, feel free to join our [Support Server](https://discord.gg/G5pEdUp)!


