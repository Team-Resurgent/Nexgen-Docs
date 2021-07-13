# vector2

vector2 module

- [unpack](#unpack)
- [lerp](#lerp)
- [invertY](#invertY)
- [invertX](#invertX)

## unpack

```lua
vector2.unpack()
```

Used to unpack vector into its 2 elements.

| Output type | Description |
| --- | --- |
| `number` | x element |
| `number` | y element |

## lerp

```lua
vector2.lerp(secondVector, alpha)
```

Used to interpolate between vector value and an other

| Output type | Description |
| --- | --- |
| `vector2` | vector |

## invertY

```lua
vector2.invertY(value)
```

Used to offset y value e.g. value - y.

@ [optional] value (number) defaults to 0

| Output type | Description |
| --- | --- |
| `vector2` | vector |

## invertX

```lua
vector2.invertX(value)
```

Used to offset y value e.g. value - x.

@ [optional] value (number) defaults to 0

| Output type | Description |
| --- | --- |
| `vector2` | vector |