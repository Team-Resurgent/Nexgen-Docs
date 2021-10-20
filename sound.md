# sound

sound module

- [load](#load)
- [play](#play)
- [stop](#stop)
- [isPlaying](#isPlaying)
- [getVolume](#getVolume)
- [setVolume](#setVolume)
- [setRepeat](#setRepeat)
- [delete](#delete)

## load

```lua
sound.load(path)
```

Used to load a sound from given path into memory. Current supported formats are [wav].

| Input | Type | Description |
| --- | --- | --- |
| `path` | `string` | path of sound to load |

| Output type | Description |
| --- | --- |
| `integer` | ID of sound, otherwise 0 |

## play

```lua
sound.play(soundId)
```

Used to start playing sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `soundId` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## stop

```lua
sound.stop(soundId)
```

Used to stop playing sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `soundId` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## isPlaying

```lua
sound.isPlaying(soundId)
```

Used to check if sound is still playing.

| Input | Type | Description |
| --- | --- | --- |
| `soundId` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## getVolume

```lua
sound.getVolume(soundId)
```

Used to get volume of sound.

| Input | Type | Description |
| --- | --- | --- |
| `soundId` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `number` | Sound volume percent 0 to 1 for left channel |
| `number` | Sound volume percent 0 to 1 for right channel |

## setVolume

```lua
sound.setVolume(soundId, percent)
```

Used to set volume of sound.

| Input | Type | Description |
| --- | --- | --- |
| `soundId` | `integer` | ID of sound |
| `percentLeft` | `number` | sound volume percent 0 to 1 for left channel |
| `percentRight` | `number` | sound volume percent 0 to 1 for right channel |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## setRepeat

```lua
sound.setRepeat(soundId, count)
```

Used to set repeat flag on sound (should be called before play).

| Input | Type | Description |
| --- | --- | --- |
| `soundId` | `integer` | ID of sound |
| `count` | `integer` | times to repeat, -1 to repeat for ever |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## delete

```lua
sound.delete(soundId)
```

Used to delete sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `soundId` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |