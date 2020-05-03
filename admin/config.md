# Config

### Description
This command is used to set various settings without needing to go through the full setup.
### Optional Arguments
`list` - This argument is used to show current server settings.

`element` - If this is used without any other argument, it will show current settings for that element.


*For configuration*

<!-- tabs:start -->
#### **Admin Roles**
## Config Element

### `admin`
## Function

**Anyone with any of these roles inherits staff permissions, but also has permission to configure server settings.**

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config admin [add/remove/list] [role]`

#### **Staff Roles**

## Config Element

### `staff`
## Function

**Anyone with any of these roles has permission to accept and deny suggestions, as well as interact with them in other ways.**

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config staff [add/remove/list] [role]`

#### **Allowed Suggestion Roles**

## Config Element

### `allowed`
## Function

**Anyone with any of these roles (or a staff/admin role) can submit suggestions. If no allowed roles are set, all members can submit suggestions.**

?> This is useful for locking suggesting to only some members of your server!

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config allowed [add/remove/list] [role]`

#### **Approved Suggestion Role**

## Config Element

### `approvedrole`
## Function

**When a member's suggestion is approved they will automatically receive this role.**

**Using** `none` **as the value will remove the approved suggestion role if there is one set.**

## Valid Inputs

**Role name, ID, or @mention**

## Usage

`config approvedrole [role]`

#### **Review Channel**

## Config Element

### `review`
## Function

**The channel where suggestions are sent immediately after submission to be reviewed by staff. (Only if the mode is set to *review*)**

## Valid Inputs

**Channel ID, name or #mention**

## Usage

`config review [channel]`

#### **Approved Suggestions Channel**

## Config Element

### `suggestions`
## Function

**The channel where approved suggestions are posted. (If the mode is set to *autoapprove* then suggestions are automatically posted here)**

## Valid Inputs

**Channel ID, name or #mention**

## Usage

`config suggestions [channel]`

#### **Denied Suggestions Channel**

## Config Element

### `denied`
## Function"

**The channel where suggestions that are denied/deleted are posted.**

**Using** `none` **as the channel will remove the denied suggestions channel if there is one set.**

## Valid Inputs

**Channel ID, name or #mention or** `none`

## Usage

`config denied [channel]`

#### **Log Channel**

## Config Element

### `logs`
## Function

**The channel where all actions taken on suggestions are logged.**

**Using** `none` **as the channel will remove the log channel if there is one set.**

## Valid Inputs

**Channel ID, name or #mention or** `none`

## Usage

`config logs [channel]`

#### **Implemented Archive Channel**

## Config Element

### `implemented`
## Function

**The channel where all suggestions that have been marked as __implemented__ using the [mark](/staff/mark.md) command are sent.**

**Using** `none` **as the channel will remove the implemented archive channel if there is one set.**

## Valid Inputs

**Channel ID, name or #mention or** `none`

## Usage

`config implemented [channel]`

#### **Suggestion Command Channel**

## Config Element

### `commands`
## Function

**The channel where the** `suggest` **command can be used. (If this is not set the suggest command can be used in any channel)**

?> This is useful for keeping suggest commands out of chat channels!

**Using** `none` **as the channel will remove the implemented archive channel if there is one set.**

## Valid Inputs

**Channel ID, name or #mention or** `none`

## Usage

`config commands [channel]`

#### **Reaction Emojis**

## Config Element

### `emojis`
## Function

**The emojis that should be reacted on approved suggestions. The defaults are 👍, 🤷, and 👎 for upvote, shrug, and downvote respectively.**

**Selecting** `disable` **for an emote disables it - meaning it won't be added to future approved suggestions.**

**The** `toggle`/`enable`/`disable` **parameters will edit the setting controlling reactions to suggestion feed posts - this is *enabled* by default.**

## Valid Inputs

**Unicode or custom emoji from the server.**

## Usage

`config emojis [upvote/shrug/downvote/toggle/enable/disable] [emoji/disable]`

#### **Notify Settings**

## Config Element

### `notify`
## Function

**The** `notify` **element specifies whether server members should be notified through DM when actions are taken on their suggestions.**

**This is *enabled* by default.**

## Valid Inputs

`enable`, `disable`, **or** `toggle`

## Usage

`config notify [enable/disable/toggle]`

#### **Suggestions Mode**

## Config Element

### `mode`
## Function

**The** `mode` **element configures the mode of suggestion handling.**

**Setting this to** `review` **will put all suggestions through the review process before sending them to the suggestions channel.**

**Setting this to** `autoapprove` **will automatically send all submitted suggestions to the suggestions feed.**

## Valid Inputs

`review` **or** `autoapprove`

## Usage

`config mode [review/autoapprove]`

#### **Auto-Clean Suggestion Channel**

## Config Element

### `cleancommands`
## Function

**This element specifies whether or not suggestion commands and responses are deleted after a few seconds.**

**This is *disabled* by default.**

?> This is useful for keeping your suggestion channel clean!

## Valid Inputs

`enable`, `disable` **or** `toggle`

## Usage

`config cleancommands [enable/disable/toggle]`

#### **Prefix**

## Config Element

### `prefix`
## Function

**The prefix that all commands start with Example: in** `.command` **the prefix is** `.`

## Valid Inputs

**Any string with no spaces**

## Usage

`config prefix [prefix]`

<!-- tabs:end -->


### Usage
```
.config (element) (additional parameters)
```
### Aliases
`serverconfig`, `cfg`, `configure`
### Required Permissions
People with **Manage Server** permission or configured admin role.
