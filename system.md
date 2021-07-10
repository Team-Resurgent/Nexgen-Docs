# system

system module

- [debugBreak](#debugBreak)
- [getTotalVirtualMemory](#getTotalVirtualMemory)
- [getFreeVirtualMemory](#getFreeVirtualMemory)
- [getTotalPhysicalMemory](#getTotalPhysicalMemory)
- [getFreePhysicalMemory](#getFreePhysicalMemory)
- [launch](#launch)

## debugBreak

```lua
system.debugBreak()
```

Used to aid debugging.

## getTotalVirtualMemory

```lua
system.getTotalVirtualMemory()
```

Used to get amount of virtual memory that is used.

| Output type | Description |
| --- | --- |
| `integer` | Total amount of virtual memory in use. |

## getFreeVirtualMemory

```lua
system.getFreeVirtualMemory()
```

Used to get amount of virtual memory that is free.

| Output type | Description |
| --- | --- |
| `integer` | Total amount of virtual memory free. |

## getTotalPhysicalMemory

```lua
system.getTotalPhysicalMemory()
```

Used to get amount of physical memory that is used.

| Output type | Description |
| --- | --- |
| `integer` | Total amount of physical memory in use. |

## getFreePhysicalMemory

```lua
system.getFreePhysicalMemory()
```

Used to get amount of physical memory that is free.

| Output type | Description |
| --- | --- |
| `integer` | Total amount of physical memory free. |

## launch

```lua
system.launch(path)
```

Used to launch a executable from given path.

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of executable to load |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |