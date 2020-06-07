# Config

### Description
Configure individual options for the bot.
### Optional Arguments
`list` - Show the server's current configuration.

`element` - The setting to change.

`...input` - The value of the setting you would like to change. Leaving this blank will show the current value.


*For configuration*

<!-- tabs:start -->
#### **Admin Roles**
## Config Element

### `admin`
## Function

**The admin role automatically inherits all staff permissions and the ability to configure server settings.**

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config admin [<add|remove|list> <role>]`

#### **Staff Roles**

## Config Element

### `staff`
## Function

**The staff roles grant permission to interact with suggestions (approve, deny, etc.).**

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config staff [<add|remove|list> <role>]`

#### **Allowed Suggestion Roles**

## Config Element

### `allowed`
## Function

**Anyone with these roles can sumbit suggestions. If this is left blank, all members may submit suggestions.**

?> This is useful for locking the ability to make suggestions to specific server members.

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config allowed [<add|remove|list> <role>]`

#### **Blocked Roles**

## Config Element

### `blocked`
## Function

**Anyone with these roles cannot use the bot, unless they have a staff/admin role.**

?> This works similarly to the [blacklist](staff/blacklist) command, but blacklists a role instead of a user.

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config blocked [<add|remove|list> <role>]`

#### **Approved Suggestion Role**

## Config Element

### `approvedrole`
## Function

**When a member's suggestion is approved, they will automatically receive this role.**

**Using** `none` **as the value will remove the approved suggestion role if one is set.**

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config approvedrole [role]`

#### **Suggestion Submitted Mention Role**

## Config Element

### `pingrole`
## Function

**When a member submits a suggestion (in the review mode) this role will be mentioned in the suggestion review channel.**

**Using** `none` **as the value will remove the suggestion submitted mention role if one is set.**

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config pingrole [role]`

#### **Review Channel**

## Config Element

### `review`
## Function

**The channel where suggestions are sent to be reviewed by server staff. (This channel will only be used if the mode is set to *review*)**

## Valid Inputs

**Channel name, ID or #mention**

## Usage

`config review [channel]`

#### **Approved Suggestions Channel**

## Config Element

### `suggestions`
## Function

**The channel is where approved suggestions will be sent. (If the mode is set to *autoapprove*, suggestions will automatically be posted here)**

## Valid Inputs

**Channel name, ID or #mention**

## Usage

`config suggestions [channel]`

#### **Denied Suggestions Channel**

## Config Element

### `denied`
## Function"

**The channel where suggestions that are denied or deleted are posted.**

**Using** `none` **will remove the denied suggestions channel if one is set.**

## Valid Inputs

**Channel name, ID, #mention or** `none`

## Usage

`config denied [channel]`

#### **Log Channel**

## Config Element

### `logs`
## Function

**The channel where all actions taken on suggestions are logged.**

**Using** `none` **will remove the log channel if one is set.**

## Valid Inputs

**Channel name, ID, #mention or** `none`

## Usage

`config logs [channel]`

#### **Implemented Archive Channel**

## Config Element

### `implemented`
## Function

**The channel where all suggestions that have been marked as __implemented__ are sent.**

**Using** `none` **will remove the implemented suggestions channel if one is set.**

## Valid Inputs

**Channel name, ID, #mention or** `none`

## Usage

`config implemented [channel]`

#### **Suggestion Command Channel**

## Config Element

### `commands`
## Function

**The channel where the** `suggest` **command can be used. (If this is not set, the** `suggest` **command can be used in any channel)**

?> This is useful for keeping suggest commands out of chat channels!

**Using** `none` **will remove the suggestion channel if one is set.**

## Valid Inputs

**Channel name, ID, #mention or** `none`

## Usage

`config commands [channel]`

#### **Reaction Emojis**

## Config Element

### `emojis`
## Function

**The reactions that will be added to approved suggestions. By default, 👍, 🤷 and 👎 will be used.**

**Selecting** `disable` **will disable it, meaning it will not be added to approved suggestions in the future.**

## Valid Inputs

**Unicode or custom emoji from the server.**

## Usage

`config emojis [<upvote|shrug|downvote|toggle|enable|disable>] [emoji|disable]`

#### **Notify Settings**

## Config Element

### `notify`
## Function

**The** `notify` **element specifies whether server members will be notified when actions are taken on suggestions they have submitted.**

**This is *enabled* by default.**

## Valid Inputs

`enable`, `disable` **or** `toggle`

## Usage

`config notify [enable|disable|toggle]`

#### **Suggestions Mode**

## Config Element

### `mode`
## Function

**The** `mode` **element configures the mode of suggestion handling.**

**Setting the mode to** `review` **will send all suggestions to the review channel before sending them to the suggestions channel.**

**Setting the mode to** `autoapprove` **will automatically send all submitted suggestions directly to the suggestions feed.**

## Valid Inputs

`review` **or** `autoapprove`

## Usage

`config mode [review|autoapprove]`

#### **Auto-Clean Suggestion Channel**

## Config Element

### `cleancommands`
## Function

**This will automatically deletes suggestion commands and the bot's response shortly after running the command.**

**This is *disabled* by default.**

?> This is useful for keeping your suggestion channel clean!

## Valid Inputs

`enable`, `disable` **or** `toggle`

## Usage

`config cleancommands [enable|disable|toggle]`

#### **Locale**

## Config Element

### `locale`
## Function

**The locale config element allows you to set the language in which server responses and feed messages will be shown in.**

**Not specifying a locale will show the list of available locales and the currently selected locale.**

## Valid Inputs

**Any locale name**

## Usage

`config locale [locale]`

#### **Prefix**

## Config Element

### `prefix`
## Function

**The prefix that will be used for all of Suggester's commands**

**The default prefix is** `.`

## Valid Inputs

**Any string with no spaces**

## Usage

`config prefix [prefix]`

<!-- tabs:end -->


### Usage
```
.config <element> [additional parameters]
```
### Aliases
`serverconfig`, `cfg`, `configure`
### Required Permissions
The user must have **Manage Server** or the configured admin role.
