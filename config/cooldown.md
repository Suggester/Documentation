# Configuration Element: Suggestion Cooldown 

### What is it for?
This element defines how long will users have to wait before being able to send a suggestion again 

### Usage
Configure the suggestion cooldown using `.config cooldown [time]`

!> Your configured cooldown cannot be lower than the internal cooldown for the `suggest` command which is currently set to **20 seconds**. Trying to set the cooldown to any number lower than this number will throw an error.

### Aliases
`suggestcooldown`, `cd` and `suggestcd`

### Accepted Imputs
See the table below for more information on how to format durations:

| Name     | Shortcut |
|:--------:|:--------:|
| seconds  | s        |
| minutes  | m        |
| hours    | h        |
| days     | d        |

> **Examples:**
> Using `.config cooldown 25s` will set the suggestion cooldown to **25 seconds**\
> Using `.config cooldown 3h` will set the cooldown to **3 hours**

?> Members with staff or admin permissions are not affected by this cooldown.
