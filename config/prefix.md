# Configuration Element: Prefix

### What is it for?
The specific character or group of characters (usually a symbol) used to invoke a bot command. 

### Default Value
By default, the prefix is `.` (a dot) which means commands will be used like this: `.command` 

?> Pinging the bot (`@Suggester#8366`) will always work as a prefix.

### Usage
Set up the prefix using `.config prefix [new prefix]` or `.prefix [new prefix]`

### Accepted Imputs
Any string between 1 and 20 characters 

!> It is strongly recommended to **avoid including "suggest"** or the likes in your prefix, as it can cause confusion when trying to use the bot.
