# Configuration Element: Color Change

### What is it for?
If configured, this setting defines if the color of the suggestion embed will automatically change when the number of net upvotes reaches a certain theresold. You can customize both the color and the number of **net** upvotes required for the color to change! 

### Usage
Set up the new color using `.config colorchange color [color]`\
Set up the requires theresold using `.config colorchange number [number]`

> This element supports [HEX colors](https://www.w3schools.com/colors/colors_picker.asp), [CSS colors](https://www.w3schools.com/colors/colors_w3css.asp), and more!

### Accepted Imputs
| Argument        | Valid Imput                       |
|-----------------|:---------------------------------:|
| color           | Any valid HEX or CSS color code   |
| number          | Any number greater than 0         |


?> The color will only change when the amount of **net** upvotes (downvotes - upvotes) reaches the configured theresold.

### Default Values
At **15** net upvotes, the embed color will change to [**#FFD700**](https://cdn.discordapp.com/attachments/650509356013715477/832271103966969926/background-FFD700.png?size=512).
