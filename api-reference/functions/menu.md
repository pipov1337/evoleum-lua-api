---
description: Various tricks with menu
---

# menu

## get\_alpha

Returns the menu alpha

```lua
float get_alpha()
```

**Example**

```lua
print("menu opened: ", menu.get_alpha() > 0)
```

## add\_group

Creates a group econtrol and returns it

```lua
group_t add_group(string name)
```

| Fields | Description |
| ------ | ----------- |
| name   | group name  |

#### Example

```lua
local group = menu.add_group("group")
```

## add\_checkbox

Creates a checkbox control and returns it

```lua
checkbox_t add_checkbox(string group, string name)
```

| Fields  | Description                               |
| ------- | ----------------------------------------- |
| `group` | group in which the control will be placed |
| `name`  | checkbox name                             |

**Example**

```lua
local checkbox_item = menu.add_checkbox("group", "checkbox")
```



### add\_selection

Creates a selection control and returns it

```lua
selection_t add_selection(string group, string name, table items)
```

|         | Description    |
| ------- | -------------- |
| `group` | group name     |
| `name`  | selection name |
| `items` | array of items |

**Example**

```lua
local selection_item = menu.add_selection("group", "select", {"element1", "element2", "element3"})
```

### add\_slider

Creates a slider control and returns it

```java
slider_t add_slider(string group, string name, int digits, double min, double max, double currentValue)
```

|                | Description                      |
| -------------- | -------------------------------- |
| `group`        | group name                       |
| `name`         | selection name                   |
| `min`          | minimum slider value             |
| `max`          | maximum slider value             |
| `currentValue` | current slider value (0.0 - 1.0) |

**Example**

```
local slider_item = menu.add_slider("group", "slider", 1, 0, 10, 0.5)
```

### add\_text\_input

Creates a text input control and returns it

```java
text_input_t add_text_input(string group, string name, string input)
```

| Fields  | Description    |
| ------- | -------------- |
| `group` | group name     |
| `name`  | selection name |
| `input` | text input     |

#### Example

```lua
local text_input_item = menu.add_text_input("group", "text input", "test")
```

### add\_multi\_selection

Creates a multi selection control and returns it

```lua
multi_selection_t add_multi_selection(string group, string name, table items)
```

| Fields  | Description    |
| ------- | -------------- |
| `group` | group name     |
| `name`  | control name   |
| `items` | array of items |

**Example**

```lua
local multi_selection_item = menu.add_multi_selection("group", "select", {"element1", "element2", "element3"})
```
