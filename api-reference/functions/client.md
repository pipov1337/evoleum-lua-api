---
description: Various tricks with client
---

# client

## get\_fps

Returns the client's frames per second

```lua
int get_fps()
```

**Example**

```lua
print(client.get_fps())
```

### get\_unix\_time <a href="#get_unix_time" id="get_unix_time"></a>

Returns the current unix timestamp

```lua
int get_unix_time()
```

**Example**

```lua
print(client.get_unix_time())
```

## is\_singleplayer

Returns the player location

```lua
bool is_singleplayer()
```

**Example**

```lua
print(client.is_singleplayer())
```

## get\_partial\_ticks

#### Returns the ticks

```lua
float get_partial_ticks()
```

## Example

```lua
print(client.get_partial_ticks())
```

## random\_float

#### Returns random float

```lua
float random_float(float min, float max)
```

## Example

```lua
print(client.random_float(10, 50))
```

## random\_int

#### Returns random int

```lua
int random_float(int min, int max)
```

## Example

```lua
print(client.random_int(10, 50))
```

## print

Sending a local message

```lua
function print(string message)
```

## Example

```lua
client.print("Test Message")
```
