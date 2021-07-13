# vector3

vector3 module

- [new](#new)
- [unpack](#unpack)
- [lerp](#lerp)
- [invertY](#invertY)
- [invertX](#invertX)
- [dot](#dot)
- [cross](#cross)
- [normal](#normal)

## new

```lua
vector3.new(x, y, z)
```

Used to create a new vector3.

| Input | Type | Description |
| --- | --- | --- |
| `x` | `number` | x element |
| `y` | `number` | y element |
| `z` | `number` | z element |

| Output type | Description |
| --- | --- |
| `vector3` | vector |

## unpack

```lua
vector3.unpack()
```

Used to unpack vector into its 3 elements.

| Output type | Description |
| --- | --- |
| `number` | x element |
| `number` | y element |
| `number` | z element |

## lerp

```lua
vector3.lerp(secondVector, alpha)
```

Used to interpolate between vector value and an other

| Output type | Description |
| --- | --- |
| `vector3` | vector |

## invertY

```lua
vector3.invertY(value)
```

Used to offset y value e.g. value - y.

@ [optional] value (number) defaults to 0

| Output type | Description |
| --- | --- |
| `vector3` | vector |

## invertX

```lua
vector3.invertX(value)
```

Used to offset x value e.g. value - x.

@ [optional] value (number) defaults to 0

| Output type | Description |
| --- | --- |
| `vector3` | vector |

## dot

```lua
vector3.dot(secondVector)
```

Used to calculate dot product of vector value and an other

| Output type | Description |
| --- | --- |
| `vector3` | vector |

## cross

```lua
vector3.cross(secondVector)
```

Used to calculate cross of vector value and an other

| Output type | Description |
| --- | --- |
| `vector3` | vector |

## normal

```lua
vector3.normal(vector3)
```

Used to normalize a vector3.

| Output type | Description |
| --- | --- |
| `vector3` | normalized vector |