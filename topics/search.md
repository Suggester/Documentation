# Searching Suggestions

Servers with a high amount of suggestions can get messy, making finding a specific suggestion based on its attributes much more complicated then its worth. Our latest release comes with a great and long requested feature: a search command! You'll be able to go through your suggestion feed manually by specifying search parameters to narrow results. This command is rather complex so we'll dive into it below.

### Usage
Use `.search <parameters separated by a space>` in any channel the bot can read and send messages in.

?> There is no limit on how many search parameters you can include. 

### Parameters and Syntax 

| Name                      | Syntax                                      |  Explanation             |
|:------------------------:|:--------------------------------------------:|:---------------------------:|
| Suggestion Status        | `status:approved/denied/review`              |  Only contains suggestions with the selected internal status |
| Marked Status            | `mark:done/working/consideration/no/default` |  Only contains suggestions [marked](/staff/mark.md) as the selected status
| Vote Count               | `votes>(number)` or `votes<(number)`         |  Only contains suggestions with more than X upvotes |
| Author                   | `author:(User ID)`                           |  Only contains suggestions sent by a specific user |
| Approved or denied by    | `staff:(User ID)`                            |  Only contains suggestions approved by a specific user | 
| Time                     | `time>(date)` or `time<(date)`               |  Only contains suggestions sent in the provided period of time |
| Content                  | `content:(string)`                           |  Only contains suggestions with the string in them |

### Examples

Using `.search status:approved votes>12 content:"memes"` will return any approved suggestion with more than 12 upvotes and that contains "memes"\
Using `.search mark!working author:123456789987654321 content!"water"` will return any suggestion **not** marked as "Working", sent by the user that has the 123456789987654321 ID and that does not contains "water" 


### Operators
The above examples support multiple operators to narrow the search results:

| Operator | Meaning      |
|:--------:|:------------:|
| `:`      | equal to     |
| `>`      | greater than |
| `<`      | less than    |
| `!`      | not          |

?> You can use quotes around strings to include spaces.


> Don't hesitate to join our [support server](https://suggester.js.org/support) if you need assistance about this rather complex implementation!
