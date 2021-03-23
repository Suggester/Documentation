# Searching Suggestions

Servers with a high amount of suggestions can get messy, making finding a specific suggestion based on its attributes much more complicated then its worth. Our latest release comes with a great and long requested feature: a search command! You'll be able to go through your suggestion feed manually by specifying search parameters to narrow results. This command is rather complex so we'll dive into it below.

### Usage
Use `.search <parameters separated by a space>` in any channel the bot can read & send messages in

?> There is no limit on how many search parameters you can include. 

### Parameters and Syntax 

| Name                      | Syntax                                   | Example   | Explanation             |
|:------------------------:|:--------------------------------------------:|:------------:|:---------------------------:|
| Suggestion Status | `status:approved/denied/review` | `status:approved` | Only contains approved suggestions |
| Marked Status | `mark:done/working/consideration/no/default` | `mark:working` | Only contains suggestions [marked](staff/mark.md) as "Working"
| Vote Count | `votes>(number)` or `votes<(number)` | `votes>30` | Only contains suggestions with more than 30 upvotes |
| Author | `author:(User ID)` | `author:327887845270487041` | Only contains suggestions sent by the user 327887845270487041 |
| Approved or denied by | `staff:(User ID)` | `staff:373912954057392138` | Only contains suggestions approved by user 327887845270487041 | 
| Time | `time>(date)` or `time<(date)`  | ` time<8h` | Only contains suggestions sent in the last 8 hours |
| Content | `content:(string)` | `content:"nice`| Only contains suggestions with the word "nice" in them |


### Operators
The above examples support multiple operators to narrow the search results:

| Operator | Meaning      |
|:--------:|:------------:|
| `:`      | equal to     |
| `>`      | greater than |
| `<`      | less than    |
| `!`      | not          |

?> You can use quotes around strings to include spaces


> Don't hesitate to join our [support server](https://suggester.js.org/support) if you need assistance about this rather complex implementation!
