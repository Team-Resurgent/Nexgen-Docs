# controller

controller module

- [getButtonStateAndValue](#getButtonStateAndValue)
- [isButtonDown](#isButtonDown)
- [isButtonHeld](#isButtonHeld)
- [isButtonUp](#isButtonUp)
- [getButtonValue](#getButtonValue)
- [Button](#Button)

## getButtonStateAndValue

```lua
controller.getButtonStateAndValue(port, buttonId)
```

Used to get controller button state and value.

| Input | Type | Description |
| --- | --- | --- |
| `port` | `integer` | controller port |
| `buttonId` | `integer` | controller button |

| Output type | Description |
| --- | --- |
| `integer` | button state |
| `number` | value in range 0 to 1 |

## isButtonDown

```lua
controller.isButtonDown(port, buttonId)
```

Used to get button down state.

| Input | Type | Description |
| --- | --- | --- |
| `port` | `integer` | controller port |
| `buttonId` | `integer` | controller button |

| Output type | Description |
| --- | --- |
| `boolean` | Whether button is down or not |

## isButtonHeld

```lua
controller.isButtonHeld(port, buttonId)
```

Used to get button held down state.

| Input | Type | Description |
| --- | --- | --- |
| `port` | `integer` | controller port |
| `buttonId` | `integer` | controller button |

| Output type | Description |
| --- | --- |
| `boolean` | Whether button is being held down or not |

## isButtonUp

```lua
controller.isButtonUp(port, buttonId)
```

Used to get button button released state.

| Input | Type | Description |
| --- | --- | --- |
| `port` | `integer` | controller port |
| `buttonId` | `integer` | controller button |

| Output type | Description |
| --- | --- |
| `boolean` | Whether button has been released or not |

## getButtonValue

```lua
controller.getButtonValue(port, buttonId)
```

Used to get controller button value.

| Input | Type | Description |
| --- | --- | --- |
| `port` | `integer` | controller port |
| `buttonId` | `integer` | controller button |

| Output type | Description |
| --- | --- |
| `number` | value in range 0 to 1 |

## Button

```lua
controller.Button
```

Collection of button values to number

| Input | Type | Description |
| --- | --- | --- |
| `DpadUp` | `string` | controller Dpad Up button |


| Output type | Description |
| --- | --- |
| `integer` | 1 |
| `integer` | 2 |
| `integer` | 3 |
| `integer` | 4 |
| `integer` | 5 |
| `integer` | 6 |
| `integer` | 7 |
| `integer` | 8 |
| `integer` | 9 |
| `integer` | 10 |
| `integer` | 11 |
| `integer` | 12 |
| `integer` | 13 |
| `integer` | 14 |
| `integer` | 15 |
| `integer` | 16 |
| `integer` | 17 |
| `integer` | 18 |
| `integer` | 19 |
| `integer` | 20 |
| `integer` | 21 |
| `integer` | 22 |
