# Configuration Element: Feed Ping

### Description
This setting defines the role that is mentioned when a new suggestion is approved and sent to the suggestions feed.

### Usage
Set up the feed ping `.config feedping [role]`, setting  `none` as the role will reset the current configuration meaning no roles will be pinged.

### Aliases
`feedping`, `approvepingrole` and `feedpingrole`

### Accepted Inputs
Any role name, id or @mention

?> Suggester will need the **Mention @everyone, @here, and All Roles** permission in order to ping the configured role if is not mentionable by default.
