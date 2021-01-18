# Configuration Element: Suggestion Cooldown 

### What is it for?
This element defines how long will users have to wait before being able to send a suggestion again 

### Usage
Configure the suggestion cooldown using `.config cooldown [time]`

### Accepted Imputs
See the table below for more information on how to format durations

| Name     | Shortcut |
|:--------:|:--------:|
| seconds  | s        |
| minutes  | m        |
| hours    | h        |
| days     | d        |
| weeks    | w        |

> **Examples:**
> Using `.config cooldown 20s` will set the suggestion cooldown to **20 seconds**\
> Using `.config cooldown 6h` will set the cooldown to **6 hours**

?> Staff & admin members are exempted from this cooldown and therefore do not need to wait between suggestions
