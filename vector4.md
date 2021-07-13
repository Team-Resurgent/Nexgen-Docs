# vector4

vector4 module

- [new](#new)
- [unpack](#unpack)
- [lerp](#lerp)
- [invertY](#invertY)
- [invertX](#invertX)

## new

```lua
vector4.new(x, y, z, w)
```

Used to create a new vector4.

| Input | Type | Description |
| --- | --- | --- |
| `x` | `number` | x element |
| `y` | `number` | y element |
| `z` | `number` | z element |
| `w` | `number` | w element |

| Output type | Description |
| --- | --- |
| `vector4` | vector |

## unpack

```lua
vector4.unpack()
```

Used to unpack vector into its 4 elements.

| Output type | Description |
| --- | --- |
| `number` | x element |
| `number` | y element |
| `number` | z element |
| `number` | w element |

## lerp

```lua
vector4.lerp(secondVector, alpha)
```

Used to interpolate between vector value and an other

| Output type | Description |
| --- | --- |
| `vector4` | vector |

## invertY

```lua
vector4.invertY(value)
```

Used to offset y value e.g. value - y.

@ [optional] value (number) defaults to 0

| Output type | Description |
| --- | --- |
| `vector4` | vector |

## invertX

```lua
vector4.invertX(value)
```

Used to offset x value e.g. value - x.

@ [optional] value (number) defaults to 0

| Output type | Description |
| --- | --- |
| `vector4` | vector |