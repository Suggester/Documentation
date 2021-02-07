# Configuration Element: In-Channel Suggestion Submission (ICSS)

### What is it for?
This setting controls whether or not users can submit suggestions by sending a message in the configured suggestions feed channel.

### Usage
Set up ICSS using `.config sendinchannel on/off/toggle`

### Accepted Imputs
Either `on`, `off` or `toggle`

?> Other bots' & system messages are ignored and will not be converted into a suggestion, regardless of your ICSS settings.

!> Messages from blocked users will be deleted if ICSS is enabled.
