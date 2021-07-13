# color4

color4 module

- [new](#new)
- [unpack](#unpack)
- [lerp](#lerp)

## new

```lua
color4.new(r, g, b, a)
```

Used to create a new color4.

| Input | Type | Description |
| --- | --- | --- |
| `r` | `number` | r element in range of 0 to 1 |
| `g` | `number` | g element in range of 0 to 1 |
| `b` | `number` | b element in range of 0 to 1 |
| `a` | `number` | a element in range of 0 to 1 |

| Output type | Description |
| --- | --- |
| `color4` | color |

## unpack

```lua
color4.unpack()
```

Used to unpack color into its 4 elements.

| Output type | Description |
| --- | --- |
| `number` | r element |
| `number` | g element |
| `number` | b element |
| `number` | a element |

## lerp

```lua
color4.lerp(secondColor, alpha)
```

Used to interpolate between color value and an other

| Output type | Description |
| --- | --- |
| `color4` | color |