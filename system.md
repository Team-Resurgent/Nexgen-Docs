# system

system module

- [debugBreak](#debugBreak)
- [getTotalVirtualMemory](#getTotalVirtualMemory)
- [getFreeVirtualMemory](#getFreeVirtualMemory)
- [getTotalPhysicalMemory](#getTotalPhysicalMemory)
- [getFreePhysicalMemory](#getFreePhysicalMemory)
- [refreshDrives](#refreshDrives)
- [getDrives](#getDrives)
- [getFiles](#getFiles)
- [getDirectories](#getDirectories)
- [launch](#launch)
- [systemIsXboxOG](#systemIsXboxOG)
- [systemIsXbox360](#systemIsXbox360)
- [systemIsXboxOne](#systemIsXboxOne)
- [systemIsWindows](#systemIsWindows)
- [systemGetXboxOGTrayState](#systemGetXboxOGTrayState)
- [registerCallback](#registerCallback)
- [unregisterCallback](#unregisterCallback)

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

## refreshDrives

```lua
system.refreshDrives()
```

Used to get refresh mounted drives.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## getDrives

```lua
system.getDrives()
```

Used to get an array of mounted drives.

| Output type | Description |
| --- | --- |
| `stringArray` | Collection of drives |

## getFiles

```lua
system.getFiles(path)
```

Used to get an array of files in a given path.

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path to search |

| Output type | Description |
| --- | --- |
| `stringArray` | Collection of files |

## getDirectories

```lua
system.getDirectories(path)
```

Used to get an array of directories in a given path.

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path to search |

| Output type | Description |
| --- | --- |
| `stringArray` | Collection of directories |

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

## systemIsXboxOG

```lua
system.systemIsXboxOG()
```

Used to check if nexgen is running on Xbox OG.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## systemIsXbox360

```lua
system.systemIsXbox360()
```

Used to check if nexgen is running on Xbox 360.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## systemIsXboxOne

```lua
system.systemIsXboxOne()
```

Used to check if nexgen is running on Xbox One.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## systemIsWindows

```lua
system.systemIsWindows()
```

Used to check if nexgen is running on Windows.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## systemGetXboxOGTrayState

```lua
system.systemGetXboxOGTrayState()
```

Used to Get the states of the DVD Drive on Xbox OG.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## registerCallback

```lua
system.registerCallback(callbackFunction)
```

Used to register a callback fnction.

| Input | Type | Description |
| --- | --- | --- |
| `callbackFunction` | `function` | function to be called on refresh |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## unregisterCallback

```lua
system.unregisterCallback(callbackFunction)
```

Used to unregister a callback fnction.

| Input | Type | Description |
| --- | --- | --- |
| `unregisterCallback` | `function` | function to be removed on refresh |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |