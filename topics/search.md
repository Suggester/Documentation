# Searching Suggestions

Servers with a high amount of suggestions can get messy, which makes it hard to find a specific suggestion based on its attributes (like its author or content). With the search command, you're able to browse your suggestion feed by specifying search parameters to narrow down results.

### Usage
Use `.search <parameters separated by a space>` in any channel the bot can read and send messages in. You can include as many search parameters as you want. 

### Parameters and Syntax

| Name                     | Syntax                                       |  Explanation                                                               | Example                             |
|:------------------------:|:--------------------------------------------:|:--------------------------------------------------------------------------:|:-----------------------------------:|
| Suggestion Status        | `status:approved/denied/review`              |  Only contains suggestions with the selected internal status               | `.search status:approved`           |
| Marked Status            | `mark:done/working/consideration/no/default` |  Only contains suggestions [marked](/staff/mark.md) as the selected status | `.search mark:working`              |
| Vote Count               | `votes>(number)` or `votes<(number)`         |  Only contains suggestions with more than X upvotes                        | `.search votes>15`                  |
| Author                   | `author:(user id)`                           |  Only contains suggestions sent by a specific user                         | `.search author:327887845270487041` |
| Approved or denied by    | `staff:(user id)`                            |  Only contains suggestions approved or denied by a specific user           | `.search staff:373912954057392138`  |
| Time                     | `time>(period)` or `time<(period)`           |  Only contains suggestions sent in the provided period of time             | `.search time<"1 month"`            |
| Content                  | `content:(string)`                           |  Only contains suggestions whose content match with the string             | `.search content:"bananas`          |

### More Examples
Here's some quick extra examples you might find useful:
- Using `.search status:approved votes>12 content:"memes"` will return any approved suggestion with **more than 12 upvotes** while containing "memes".
- Using `.search mark!working author:123456789987654321 content!"water"` will return any suggestion **not** marked as "Working", sent by the user that has the 123456789987654321 id and that does not contain "water".
- Using `.search time<30d` would return all suggestions sent in the last **30 days**.

?> You can use quotes around strings to include spaces (ex: "1 month").


### Operators
The above examples support multiple operators to narrow down the search results:

| Operator | Description  |
|:--------:|:------------:|
| `:`      | equal to     |
| `>`      | greater than |
| `<`      | less than    |
| `!`      | not          |