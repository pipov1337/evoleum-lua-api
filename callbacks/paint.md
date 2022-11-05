# PAINT

{% hint style="info" %}
you can call all [render.\*](https://docs.primordial.dev/api\_functions/render/) functions inside of this callback
{% endhint %}

this callback is called every frame

```
local function on_paint()
    print(client.get_fps())

    render.rect_filled(100, 100, 200, 200, color.rgb(255, 0, 0))
end

callbacks.add("render_screen", on_paint)
```
