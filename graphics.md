# graphics

graphics module

- [clear](#clear)
- [beginScene](#beginScene)
- [endScene](#endScene)
- [loadTexture](#loadTexture)
- [activateTexture](#activateTexture)
- [getTextureSize](#getTextureSize)
- [deleteTexture](#deleteTexture)
- [loadMeshCollection](#loadMeshCollection)
- [createSheetMeshCollection](#createSheetMeshCollection)
- [createPlaneXYMeshCollection](#createPlaneXYMeshCollection)
- [createMeshCollection](#createMeshCollection)
- [deleteTexture](#deleteTexture)
- [createMeshCollection](#createMeshCollection)
- [clearMesh](#clearMesh)
- [addMeshData](#addMeshData)
- [getMeshData](#getMeshData)
- [bindMesh](#bindMesh)
- [activateMesh](#activateMesh)
- [getMeshName](#getMeshName)
- [getMeshTransform](#getMeshTransform)
- [getMeshInfo](#getMeshInfo)
- [getMeshIndices](#getMeshIndices)
- [getChildMeshIndices](#getChildMeshIndices)
- [loadFont](#loadFont)
- [deleteFont](#deleteFont)
- [drawFont](#drawFont)
- [measureFont](#measureFont)
- [setModelMatrix](#setModelMatrix)
- [setViewMatrix](#setViewMatrix)
- [setProjectionMatrix](#setProjectionMatrix)
- [drawMesh](#drawMesh)
- [getWidth](#getWidth)
- [getHeight](#getHeight)
- [disableDepthTest](#disableDepthTest)
- [enableDepthTest](#enableDepthTest)
- [cullingMode](#cullingMode)
- [enableLights](#enableLights)
- [disableLights](#disableLights)
- [enableLight](#enableLight)
- [disableLight](#disableLight)
- [setAmbientLight](#setAmbientLight)
- [setViewport](#setViewport)
- [enableScissor](#enableScissor)
- [disableScissor](#disableScissor)
- [disableFog](#disableFog)
- [enableLinearFog](#enableLinearFog)
- [enableExponentialFog](#enableExponentialFog)
- [enableExponentialSquaredFog](#enableExponentialSquaredFog)
- [setColorTint](#setColorTint)
- [enableBlend](#enableBlend)
- [disableBlend](#disableBlend)
- [drawNinePatch](#drawNinePatch)
- [swapBuffers](#swapBuffers)
- [DepthOp](#DepthOp)
- [CullingMode](#CullingMode)
- [BlendOp](#BlendOp)
- [BlendFactor](#BlendFactor)

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

## getTextureSize

```lua
graphics.getTextureSize(textureId)
```

Measures font message size.

| Input | Type | Description |
| --- | --- | --- |
| `textureId` | `integer` | ID of texture |

| Output type | Description |
| --- | --- |
| `integer` | width |
| `integer` | height |

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
| `width` | `number` | width |
| `height` | `number` | height |
| `rows` | `number` | rows |
| `cols` | `number` | cols |

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
| `width` | `number` | width |
| `height` | `number` | height |
| `rows` | `number` | rows |
| `cols` | `number` | cols |

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

## bindMesh

```lua
graphics.bindMesh(meshCollectionId, meshId)
```

Used to bind mesh in memory to the GPU.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## activateMesh

```lua
graphics.activateMesh(meshCollectionId, meshId)
```

Used to activate mesh when about to draw a mesh.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |
| `meshId` | `integer` | ID of mesh |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

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

## getMeshInfo

```lua
graphics.getMeshInfo(meshCollectionId, meshId)
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

## getMeshIndices

```lua
graphics.getMeshIndices(meshCollectionId)
```

Used to get collecyion of mesh ID's from a given mesh collection.

| Input | Type | Description |
| --- | --- | --- |
| `meshCollectionId` | `integer` | ID of mesh collection |

| Output type | Description |
| --- | --- |
| `indexArray` | Collection of mesh ID's |

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

## deleteFont

```lua
graphics.deleteFont(fontId)
```

Used to unbind font from GPU and remove from memory.

| Input | Type | Description |
| --- | --- | --- |
| `fontId` | `integer` | ID of font |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

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

Draws current active mesh and texture, with given index pffset and count.

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

## disableDepthTest

```lua
graphics.disableDepthTest()
```

Disables depth testing

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableDepthTest

```lua
graphics.enableDepthTest()
```

Enables depth testing

| Input | Type | Description |
| --- | --- | --- |
| `depthOp` | `integer` | depth operation |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## cullingMode

```lua
graphics.cullingMode(mode)
```

Enables culling

| Input | Type | Description |
| --- | --- | --- |
| `cullingMode` | `integer` | culling mode |

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

## disableLights

```lua
graphics.disableLights()
```

Disables lights

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableLight

```lua
graphics.enableLight(lightId, position, distance, color)
```

Enables light

| Input | Type | Description |
| --- | --- | --- |
| `lightId` | `integer` | ID of light |
| `position` | `vector3` | position |
| `distance` | `number` | distance |
| `color` | `color4` | color |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## disableLight

```lua
graphics.disableLight(lightId)
```

Disable light

| Input | Type | Description |
| --- | --- | --- |
| `lightId` | `integer` | ID of light |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## setAmbientLight

```lua
graphics.setAmbientLight(color)
```

Sets ambient light

| Input | Type | Description |
| --- | --- | --- |
| `color` | `color3` | color |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## setViewport

```lua
graphics.setViewport(x, y, width, height)
```

Sets current viewport

| Input | Type | Description |
| --- | --- | --- |
| `x` | `number` | x position |
| `y` | `number` | y position |
| `width` | `number` | width |
| `height` | `number` | height |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableScissor

```lua
graphics.enableScissor(x, y, width, height)
```

Enables scissor mode

| Input | Type | Description |
| --- | --- | --- |
| `x` | `number` | x position |
| `y` | `number` | y position |
| `width` | `number` | width |
| `height` | `number` | height |

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

## enableLinearFog

```lua
graphics.enableLinearFog(color, fogStart, fogEnd)
```

Enables linear fog

| Input | Type | Description |
| --- | --- | --- |
| `color` | `color3` | fog color |
| `fogStart` | `number` | fog start value |
| `fogEnd` | `number` | fog end value |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableExponentialFog

```lua
graphics.enableExponentialFog(color, density)
```

Enables exponential fog

| Input | Type | Description |
| --- | --- | --- |
| `color` | `color3` | fog color |
| `density` | `number` | fog density |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableExponentialSquaredFog

```lua
graphics.enableExponentialSquaredFog(color, density)
```

Enables exponential squared fog

| Input | Type | Description |
| --- | --- | --- |
| `color` | `color3` | fog color |
| `density` | `number` | fog density |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## setColorTint

```lua
graphics.setColorTint(color)
```

Sets color tint

| Input | Type | Description |
| --- | --- | --- |
| `color` | `color4` | color |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## enableBlend

```lua
graphics.enableBlend(blendOp, sFactor, dFactor)
```

Enables blending

| Input | Type | Description |
| --- | --- | --- |
| `blendOp` | `integer` | blend operarton |
| `sFactor` | `integer` | source blend factor |
| `dFactor` | `integer` | dest blend factor |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## disableBlend

```lua
graphics.disableBlend()
```

Disables blending

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## drawNinePatch

```lua
graphics.drawNinePatch(textureId, position, width, height, cornerPercentX, cornerPercentY)
```

Draws nine patch mesh

| Input | Type | Description |
| --- | --- | --- |
| `textureId` | `integer` | index offset |
| `position` | `vector3` | position |
| `width` | `number` | width |
| `height` | `number` | height |
| `cornerPercentX` | `number` | X axis corner percentage of width |
| `cornerPercentY` | `number` | Y axis corner percentage of height |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## swapBuffers

```lua
graphics.swapBuffers()
```

Swaps current render buffer.

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## DepthOp

```lua
graphics.DepthOp['DepthOpId']
```


Collection of DepthOp Id values to number. Example:


| Input | Type | Description |
| --- | --- | --- |
| `Never` | `string` | = 0 |
| `Less` | `string` | = 1 |
| `Equal` | `string` | = 2 |
| `LessEqual` | `string` | = 3 |
| `Greater` | `string` | = 4 |
| `NotEqual` | `string` | = 5 |
| `GreaterEqual` | `string` | = 6 |
| `Always` | `string` | = 7 |

## CullingMode

```lua
graphics.CullingMode['CullingModeId']
```


Collection of CullingMode Id values to number. Example:


| Input | Type | Description |
| --- | --- | --- |
| `None` | `string` | = 0 |
| `Front` | `string` | = 1 |
| `Back` | `string` | = 2 |


## BlendOp

```lua
graphics.BlendOp['BlendOpId']
```


Collection of BlendOp Id values to number. Example:


| Input | Type | Description |
| --- | --- | --- |
| `Add` | `string` | = 0 |
| `Subtract` | `string` | = 1 |
| `InvSubtract` | `string` | = 2 |


## BlendFactor

```lua
graphics.BlendFactor['BlendFactorId']
```


Collection of BlendFactor Id values to number. Example:


| Input | Type | Description |
| --- | --- | --- |
| `Zero` | `string` | = 0 |
| `One` | `string` | = 1 |
| `SrcColor` | `string` | = 2 |
| `OneMinusSrcColor` | `string` | = 3 |
| `DstColor` | `string` | = 4 |
| `OneMinusDstColor` | `string` | = 5 |
| `SrcAlpha` | `string` | = 6 |
| `OneMinusSrcAlpha` | `string` | = 7 |
| `DstAlpha` | `string` | = 8 |
| `OneMinusDstAlpha` | `string` | = 9 |
| `ConstantColor` | `string` | = 10 |
| `OneMinusConstantColor` | `string` | = 11 |
| `ConstantAlpha` | `string` | = 12 |
| `OneMinusConstantAlpha` | `string` | = 13 |
| `AlphaSaturate` | `string` | = 14 |
