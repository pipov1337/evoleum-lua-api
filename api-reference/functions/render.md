---
description: Various tricks with render
---

# render

create\_font

```lua
font_t create_font(string name, int size, bool custom)
```

## Example

```lua
local font = render.create_font("Arial", 16, false)
```

## text

```lua
function text(font_t font, string text, float x, float y, int color)
```

## Example

```lua
local font = render.create_font("Arial", 16, false)

render.text(font, "Test", 10, 10, color.rgb(255, 255, 255))
```

## rect

```lua
function rect(float x, float y, float width, float height, int color)
```

## Example

```lua
render.rect(10, 10, 50, 50, color.rgb(255, 255, 255))
```

## rect\_filled

```lua
function rect_filled(float x, float y, float width, float height, int color)
```

## Example

```lua
render.rect_filled(10, 10, 50, 50, color.rgb(255, 255, 255), 6)
```

## rect\_gradient

```lua
function rect_filled(float x, float y, float width, float height, int color, int color2, int color3, int color4)
```

## Example

```lua
render.rect_gradient(10, 10, 50, 50, color.rgb(255, 255, 255), color.rgb(255, 255, 255), color.rgb(255, 0, 0), color.rgb(255, 0, 0))
```

## rect\_fade

```lua
function rect_fade(float x, float y, float width, float height, int color, int radius)
```

## Example

```lua
render.rect_fade(10, 10, 50, 50, color.rgb(255, 255, 255), 6)
```

## line

```lua
function line(float x, float y, float width, float height, int color)
```

## Example

```lua
render.line(10, 10, 50, 50, color.rgb(255, 255, 255))
```

