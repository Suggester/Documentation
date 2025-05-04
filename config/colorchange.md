# Configuration Element: Color Change

### Description
Automatically update the color of the embed when the number of **net** upvotes reaches a certain threshold. You can customize both the color and the number of **net** upvotes required for the color to change.

### Usage
Set up the new color using `.config colorchange color [color]`\
Set up the requires theresold using `.config colorchange number [number]`

### Accepted Inputs
| Argument        | Valid Imput                       |
|-----------------|:---------------------------------:|
| color           | Any valid HEX or CSS color code   |
| number          | Any number greater than 0         |


?> The color will only change when the amount of **net** upvotes (downvotes - upvotes) reaches the configured theresold.

### Default Values
At **15** net upvotes, the embed color will change to a gold tint ([#FFD700](https://singlecolorimage.com/get/FFD700/250x250)).