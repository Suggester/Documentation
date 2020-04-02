# Config
---
### Description
This command is used to set various settings without needing to go through the full setup.
### Optional Arguments
`list` - This argument is used to show current server settings.

`element` - If this is used without any other argument, it will show current settings for that element.


*For configuration*

<!-- tabs:start -->
#### **admin**
# Config Element
---

# Function
---
Anyone with this role inherits staff permissions, but also has permission to configure server settings.

# Valid Inputs
---
Role name, ID, or @mention

# Usage
---
`config admin [add/remove/list] [role]`

#### **staf**

# Config Element
---
**admin**
# Function
---


# Valid Inputs
---


# Usage
---
``

<!-- tabs:end -->




### Usage
```
.config (element) (additional parameters)
```
### Aliases
`serverconfig`, `cfg`, `configure`
### Required Permissions
People with **Manage Server** permission or configured admin role.