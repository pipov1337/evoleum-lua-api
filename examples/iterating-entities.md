---
description: Useful information
---

# Iterating Entities

```lua
local function on_update()
    for _, entity in pairs(world.get_loaded_entity_list()) do 
	print(world.get_name(entity))
    end
end

callbacks.add("update", on_update)
```
