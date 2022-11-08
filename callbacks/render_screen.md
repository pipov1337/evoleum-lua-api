---
description: Useful information
---

# ⚙ render\_screen

{% hint style="info" %}
you can call all [render.\*](../examples/iterating-entities.md) functions inside of this callback
{% endhint %}

this callback is called every frame

```lua
local function on_paint()
    print(client.get_fps())

    render.rect_filled(10, 10, 200, 200, color.rgb(255, 0, 0))
end

callbacks.add("render_screen", on_paint)
```
