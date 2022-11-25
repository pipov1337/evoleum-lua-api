---
description: Various tricks with user information
---

# user

{% code title="getting user info" %}
```lua
local user_name = profile.get_username() -- get cheat nickname
local user_uid = profile.get_uid() -- get cheat uid
```
{% endcode %}

```lua
print(string.format("i`m - %s my uid - %s", user_name, user_uid))
```
