# Configuration Element: Review Ping

### Description
This element allows you to define a role that will be mentioned when a new suggestion is submitted for review.

### Usage
Set up a pinged role using `.config reviewping [role]`, setting `none` as the role will reset the current configuration meaning no role will be pinged.

### Aliases
`submitping`, `reviewpingrole` and `submitpingrole`

### Accepted Inputs
Any role name, id or @mention

?> Suggester will need the **Mention @everyone, @here, and All Roles** permission in order to ping the configured role if it is not mentionable by default.
