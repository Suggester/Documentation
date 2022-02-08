# Searching Suggestions

Servers with a high amount of suggestions can get messy, which makes it hard to find a specific suggestion based on its attributes (like its author or conent). We've added a long requested feature: a search command! You're now able to go through your suggestion feed in the blink of an eye by specifying search parameters to narrow down results. This command is rather complex so we'll dive into it below.

### Usage
Use `.search <parameters separated by a space>` in any channel the bot can read and send messages in.

?> You can include as many search parameters as you want. 

### Parameters and Syntax 

| Name                     | Syntax                                       |  Explanation                                                               |
|:------------------------:|:--------------------------------------------:|:--------------------------------------------------------------------------:|
| Suggestion Status        | `status:approved/denied/review`              |  Only contains suggestions with the selected internal status               |
| Marked Status            | `mark:done/working/consideration/no/default` |  Only contains suggestions [marked](/staff/mark.md) as the selected status |
| Vote Count               | `votes>(number)` or `votes<(number)`         |  Only contains suggestions with more than X upvotes                        |
| Author                   | `author:(user id)`                           |  Only contains suggestions sent by a specific user                         |
| Approved or denied by    | `staff:(user id)`                            |  Only contains suggestions approved by a specific user                     | 
| Time                     | `time>(date)` or `time<(date)`               |  Only contains suggestions sent in the provided period of time             |
| Content                  | `content:(string)`                           |  Only contains suggestions with the string in them                         |

### Examples

Using `.search status:approved votes>12 content:"memes"` will return any approved suggestion with more than 12 upvotes and that contains "memes"\
Using `.search mark!working author:123456789987654321 content!"water"` will return any suggestion **not** marked as "Working", sent by the user that has the 123456789987654321 id and that does not contain "water" 


### Operators
The above examples support multiple operators to narrow down the search results:

| Operator | Meaning      |
|:--------:|:------------:|
| `:`      | equal to     |
| `>`      | greater than |
| `<`      | less than    |
| `!`      | not          |

?> You can use quotes around strings to include spaces.

> Don't hesitate to join our [support server](https://suggester.js.org/support) if you need assistance about this rather complex implementation.
