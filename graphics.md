# graphics

graphics module

- [clear](#clear)
- [beginScene](#beginScene)
- [beginScene](#beginScene)

## clear

```lua
graphics.clear(clearDepth, depthValue, clearStencil, stencilValue, clearTarget, targetColor)
```

Used to clear render depth, stenil and target buffers.

| Input | Type | Description |
| --- | --- | --- |
| `clearDepth` | `boolean` | whether to clear depth or not |
| `depthValue` | `number` | depth value |
| `clearStencil` | `boolean` | whether to clear stencil or not |
| `stencilValue` | `number` | stencil value |
| `clearTarget` | `boolean` | whether to clear target or not |
| `targetColor` | `color4` | target color |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## beginScene

```lua
graphics.beginScene()
```

Used to denote start of rendering calls.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## beginScene

```lua
graphics.beginScene()
```

Used to denote end of rendering calls.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |