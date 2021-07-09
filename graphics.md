# graphics

graphics module

- [clear](#clear)
- [beginScene](#beginScene)
- [endScene](#endScene)
- [loadTexture](#loadTexture)
- [activateTexture](#activateTexture)
- [deleteTexture](#deleteTexture)
- [loadMeshCollection](#loadMeshCollection)
- [createSheetMeshCollection](#createSheetMeshCollection)
- [createPlaneXYMeshCollection](#createPlaneXYMeshCollection)
- [createMeshCollection](#createMeshCollection)
- [bindMeshCollection](#bindMeshCollection)
- [deleteTexture](#deleteTexture)

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

Used to load a texture from given path into memory and bind to the GPU. Current supported image types are [bmp, gif, hdr, jpg, pic, png, pnm, psd, tga].

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of image to load |

| Output type | Description |
| --- | --- |
| `integer` | returns id of loaded texture, otherwise 0 |

## activateTexture

```lua
graphics.activateTexture(id)
```

Used to activate texture when about to draw a mesh.

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of image to load |

| Output type | Description |
| --- | --- |
| `integer` | returns id of loaded texture, otherwise 0 |

## deleteTexture

```lua
graphics.deleteTexture(id)
```

Used to unbind texture from GPU and remove from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | id of texture |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## loadMeshCollection

```lua
graphics.loadMeshCollection(path)
```

Used to load a mesh collection from given path into memory. Current supported mesh file types are [glb, gltf, xm, obj].

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of mesh to load |

| Output type | Description |
| --- | --- |
| `integer` | returns id of loaded mesh collection, otherwise 0 |

## createSheetMeshCollection

```lua
graphics.createSheetMeshCollection(x, y, z, width, height, rows, cols)
```

Used to create a mesh collection into memory consising of a single mesh. The mesh is divided in a number of rows and columns. Each cell is an individual quad.

| Input | Type | Description |
| --- | --- | --- |
| `x` | `number` | x position |
| `y` | `number` | y position |
| `z` | `number` | z position |
| `width` | `number` | width position |
| `height` | `number` | height position |
| `width` | `number` | width position |
| `cols` | `number` | cols position |

| Output type | Description |
| --- | --- |
| `integer` | returns id of mesh collection, otherwise 0 |

## createPlaneXYMeshCollection

```lua
graphics.createPlaneXYMeshCollection(x, y, z, width, height, rows, cols)
```

Used to create a mesh collection into memory consising of a single mesh. The mesh is divided in a number of rows and columns. Each cell is connected to the next.

| Input | Type | Description |
| --- | --- | --- |
| `x` | `number` | x position |
| `y` | `number` | y position |
| `z` | `number` | z position |
| `width` | `number` | width position |
| `height` | `number` | height position |
| `width` | `number` | width position |
| `cols` | `number` | cols position |

| Output type | Description |
| --- | --- |
| `integer` | returns id of mesh collection, otherwise 0 |

## createMeshCollection

```lua
graphics.createMeshCollection()
```

Used to create a empty mesh collection in memory.

| Output type | Description |
| --- | --- |
| `integer` | returns id of mesh collection, otherwise 0 |

## bindMeshCollection

```lua
graphics.bindMeshCollection(id)
```

Used to bind mesh collection to the GPU.

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of image to load |

| Output type | Description |
| --- | --- |
| `integer` | returns id of loaded texture, otherwise 0 |

## deleteTexture

```lua
graphics.deleteTexture(id)
```

Used to unbind mesh collection from GPU and remove from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | id of mesh collection |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |