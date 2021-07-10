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

| Output type | Description |
| --- | --- |
| `integer` | ID of sound, otherwise 0 |

## play

```lua
sound.play(id)
```

Used to start playing sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## stop

```lua
sound.stop(id)
```

Used to stop playing sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## isPlaying

```lua
sound.isPlaying(id)
```

Used to check if sound is still playing.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## setRepeat

```lua
sound.setRepeat(id, count)
```

Used to set repeat flag on sound.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |
| `count` | `integer` | times to repeat, -1 to repeat for ever |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## delete

```lua
sound.delete(id)
```

Used to delete sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |