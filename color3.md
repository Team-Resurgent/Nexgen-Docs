# color3

color3 module

- [new](#new)
- [unpack](#unpack)
- [lerp](#lerp)

## new

```lua
color3.new(r, g, b)
```

Used to create a new color3.

| Input | Type | Description |
| --- | --- | --- |
| `r` | `number` | r element in range of 0 to 1 |
| `g` | `number` | g element in range of 0 to 1 |
| `b` | `number` | b element in range of 0 to 1 |

| Output type | Description |
| --- | --- |
| `color3` | color |

## unpack

```lua
color3.unpack()
```

Used to unpack color into its 3 elements.

| Output type | Description |
| --- | --- |
| `number` | r element |
| `number` | g element |
| `number` | b element |

## lerp

```lua
color3.lerp(secondColor, alpha)
```

Used to interpolate between color value and an other

| Output type | Description |
| --- | --- |
| `color3` | color |