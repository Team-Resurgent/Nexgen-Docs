# sound

sound module

- [sound](#sound)
- [sound](#sound)
- [sound](#sound)
- [sound](#sound)
- [sound](#sound)
- [sound](#sound)

## sound

```lua
sound.sound.load(path)
```

Used to load a sound from given path into memory. Current supported formats are [wav,].

| Output type | Description |
| --- | --- |
| `integer` | ID of sound, otherwise 0 |

## sound

```lua
sound.sound.play(id)
```

Used to start playing sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## sound

```lua
sound.sound.stop(id)
```

Used to stop playing sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## sound

```lua
sound.sound.isPlaying(id)
```

Used to check if sound is still playing.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## sound

```lua
sound.sound.setRepeat(id, count)
```

Used to set repeat flag on sound.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |
| `count` | `integer` | index count |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |

## sound

```lua
sound.sound.delete(id)
```

Used to delete sound from memory.

| Input | Type | Description |
| --- | --- | --- |
| `id` | `integer` | ID of sound |

| Output type | Description |
| --- | --- |
| `boolean` | Whether or not the operation succeeded |