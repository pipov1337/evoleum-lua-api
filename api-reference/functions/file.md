---
description: Various tricks with files
---

# file

## create\_folder

create a folder

```lua
file_t create_folder(string folder)
```

#### Example

```lua
file.create_folder("test")
```

## create\_file

create a file

```lua
file_t create_file(string file)
```

## Example

```lua
file.create_file("test.txt")
```

## read

```lua
function read(string path)
```

## Example

```lua
print(file.read("test.txt"))
```

## list\_files

file table

```lua
table list_files(string path)
```

## write

```lua
file.write(string path, string content)
```

## Example

```lua
file.write("test.txt", "test")
```

## exists

```
bool exists(string path)
```

## Example

```lua
print(file.exists("test.txt"))
```
