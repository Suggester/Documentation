# Configuration Element: Suggestion Cooldown

### Description
This element defines how long users will have to wait before being able to send a suggestion again.  Members with staff or admin permissions are not affected by this cooldown.

### Usage
Configure the suggestion cooldown using `.config cooldown [time]`

!> Your configured cooldown cannot be lower than the internal cooldown for the `suggest` command which is currently set to **20 seconds**. Trying to set the cooldown to any number lower than this number will throw an error.

### Aliases
`suggestcooldown`, `cd` and `suggestcd`

### Accepted Inputs
You can use "s" for seconds, "m" for minutes, "h" for hours and "d" for days.

### **Examples:**
- Using `.config cooldown 25s` will set the suggestion cooldown to **25 seconds**.\
- Using `.config cooldown 3h` will set the cooldown to **3 hours**.