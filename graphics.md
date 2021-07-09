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
- [createMeshCollection](#createMeshCollection)
- [clearMesh](#clearMesh)
- [addMeshData](#addMeshData)
- [getMeshData](#getMeshData)
- [bindMeshCollection](#bindMeshCollection)
- [getMeshCount](#getMeshCount)
- [getMeshName](#getMeshName)
- [getMeshTransform](#getMeshTransform)
- [getMeshData](#getMeshData)
- [getChildMeshIndices](#getChildMeshIndices)
- [loadFont](#loadFont)
- [drawFont](#drawFont)
- [measureFont](#measureFont)
- [setModelMatrix](#setModelMatrix)
- [setViewMatrix](#setViewMatrix)
- [setProjectionMatrix](#setProjectionMatrix)
- [drawMesh](#drawMesh)
- [getWidth](#getWidth)
- [getHeight](#getHeight)
- [disableDepth](#disableDepth)
- [enableDepth](#enableDepth)
- [enableLights](#enableLights)
- [disableights](#disableights)
- [disableScissor](#disableScissor)
- [disableFog](#disableFog)
- [disableBlend](#disableBlend)
- [getHeight](#getHeight)

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
| `integer` | ID of texture, otherwise 0 |

## activateTexture

```lua
graphics.activateTexture(textureId)
```

Used to activate texture when about to draw a mesh.

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of image to load |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## deleteTexture

```lua
graphics.deleteTexture(textureId)
```

Used to unbind texture from GPU and remove from memory.

| Input | Type | Description |
| --- | --- | --- |
| `textureId` | `integer` | ID of texture |

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
| `integer` | ID of mesh collection, otherwise 0 |

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
| `integer` | ID of mesh collection, otherwise 0 |

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
| `integer` | ID of mesh collection, otherwise 0 |

## createMeshCollection

```lua
graphics.createMeshCollection()
```

Used to create a empty mesh collection in memory.

| Output type | Description |
| --- | --- |
| `integer` | meshCollectionId of mesh collection, otherwise 0 |

## bindMeshCollection

```lua
graphics.bindMeshCollection(meshCollectionId)
```

Used to bind mesh collection to the GPU.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## deleteTexture

```lua
graphics.deleteTexture(meshCollectionId)
```

Used to unbind mesh collection from GPU and remove from memory.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## createMeshCollection

```lua
graphics.createMeshCollection()
```

Used to create a empty mesh in memory and add to a given mesh collection.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection to add to |

| Output type | Description |
| --- | --- |
| `integer` | ID of mesh, otherwise 0 |

## clearMesh

```lua
graphics.clearMesh(meshCollectionId, meshId)
```

Used to clear a mesh in memory for a given mesh collection and mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `integer` | ID of mesh, otherwise 0 |

## addMeshData

```lua
graphics.addMeshData(meshCollectionId, meshId, vertices, indicies)
```

Used to add vertices and indices to a mesh in memory for a given mesh collection and mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |
| `vertices` | `vertexArray` | collection of vertices |
@ [optional] indicies (indexArray) collection of indicies

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## getMeshData

```lua
graphics.getMeshData(meshCollectionId, meshId)
```

Used to get vertex and index arrays for a given mesh collection and mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `vertexArray` | Collection of vertices |
| `indexArray` | Collection of indicies if exists otherwise nil |

## bindMeshCollection

```lua
graphics.bindMeshCollection(meshCollectionId)
```

Used to activate mesh when about to draw a mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## getMeshCount

```lua
graphics.getMeshCount(meshCollectionId)
```

Used to get mesh copunt for a given mesh collection.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |

| Output type | Description |
| --- | --- |
| `integer` | Count of meshes |

## getMeshName

```lua
graphics.getMeshName(meshCollectionId, meshId)
```

Used to get mesh name for a given mesh collection and mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `matrix4` | transform matrix for mesh |

## getMeshTransform

```lua
graphics.getMeshTransform(meshCollectionId, meshId)
```

Used to get tranform matrix for a given mesh collection and mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `matrix4` | transform matrix for mesh |

## getMeshData

```lua
graphics.getMeshData(meshCollectionId, meshId)
```

Used to get index offset and count for a given mesh collection and mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `integer` | index offset |
| `integer` | index count |

## getChildMeshIndices

```lua
graphics.getChildMeshIndices(meshCollectionId, parentMeshId)
```

Used to get collecyion of mesh ID's from a given mesh collection and parent mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `parentMeshId` | `integer` | ID of parent mesh, 0 for root level |

| Output type | Description |
| --- | --- |
| `indexArray` | Collection of mesh ID's |

## loadFont

```lua
graphics.loadFont(path)
```

Used to load a font from given path into memory and bind to the GPU. Current supported font types are [fnt].

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of image to load |

| Output type | Description |
| --- | --- |
| `integer` | ID of font, otherwise 0 |

## drawFont

```lua
graphics.drawFont(fontId, position, message)
```

Draws font to current render buffer

| Input | Type | Description |
| --- | --- | --- |
| `fontId` | `integer` | ID of font  |
| `position` | `vector3` | position |
| `message` | `string` | message |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## measureFont

```lua
graphics.measureFont(fontId, message)
```

Measures font message size.

| Input | Type | Description |
| --- | --- | --- |
| `fontId` | `integer` | ID of font  |
| `message` | `string` | message |

| Output type | Description |
| --- | --- |
| `integer` | width |
| `integer` | height |

## setModelMatrix

```lua
graphics.setModelMatrix(modelMatrix)
```

Sets current shader model matrix.

| Input | Type | Description |
| --- | --- | --- |
| `modelMatrix` | `matrix4` | model matrix |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## setViewMatrix

```lua
graphics.setViewMatrix(viewMatrix)
```

Sets current shader view matrix.

| Input | Type | Description |
| --- | --- | --- |
| `modelMatrix` | `matrix4` | view matrix |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## setProjectionMatrix

```lua
graphics.setProjectionMatrix(projectionMatrix)
```

Sets current shader projection matrix.

| Input | Type | Description |
| --- | --- | --- |
| `modelMatrix` | `matrix4` | projection matrix |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## drawMesh

```lua
graphics.drawMesh(indexOffset, indexCount)
```

Draws current active mesh, with given index pffset and count.

| Input | Type | Description |
| --- | --- | --- |
| `indexOffset` | `integer` | index offset |
| `indexCount` | `integer` | index count |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## getWidth

```lua
graphics.getWidth()
```

Gets current render buffer width.

| Output type | Description |
| --- | --- |
| `integer` | width |

## getHeight

```lua
graphics.getHeight()
```

Gets current render buffer height.

| Output type | Description |
| --- | --- |
| `integer` | height |

## disableDepth

```lua
graphics.disableDepth()
```

Disables depth testing

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableDepth

```lua
graphics.enableDepth()
```

Enables depth testing

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableLights

```lua
graphics.enableLights()
```

Enables lights

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## disableights

```lua
graphics.disableights()
```

Disables lights

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## disableScissor

```lua
graphics.disableScissor()
```

Disables scissor

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## disableFog

```lua
graphics.disableFog()
```

Disables fog

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## disableBlend

```lua
graphics.disableBlend()
```

Disables blend

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## getHeight

```lua
graphics.getHeight()
```

Swaps current render buffer.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |