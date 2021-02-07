# Configuration Element: Color Change

### What is it for?
If configured, this setting allows you to automatically change the color of the suggestion embed when the number of net upvotes reaches a certain theresold, you can customize both the color and the number of **net** upvotes necessary to change the color! 

### Default Values
At **15** net upvotes, the embed color will change to **#FFD700**.


### Usage
Set up the new color using `.config colorchange color [color]`\
Set up the requires theresold using `.config colorchange number [number]`

> This element supports [HEX colors](https://www.w3schools.com/colors/colors_picker.asp), [CSS colors](https://www.w3schools.com/colors/colors_w3css.asp), and more!

### Accepted Imputs
| Argument              |               Valid Imput             |
|-----------------------|:-------------------------------------:|
| color                 | Any valid HEX or CSS color code       |
| number                | Any number greater than 0             |


?> The color will only change when the amount of **net** upvotes (downvotes - upvotes) reaches the configured theresold.
