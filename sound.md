# sound

sound module

- [load](#load)
- [play](#play)
- [stop](#stop)
- [isPlaying](#isPlaying)
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

## setRepeat

```lua
sound.setRepeat(soundId, count)
```

Used to set repeat flag on sound.

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