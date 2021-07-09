# graphics

graphics module

- [clear](#clear)
- [beginScene](#beginScene)
- [endScene](#endScene)
- [loadTexture](#loadTexture)

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

## endScene

```lua
graphics.endScene()
```

Used to denote end of rendering calls.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## loadTexture

```lua
graphics.loadTexture(path)
```

Used to load a texture from given path. Current supported image types are [bmp, gif, hdr, jpg, pic, png, pnm, psd, tga].

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of image to load |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |