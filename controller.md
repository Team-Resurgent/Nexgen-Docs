# controller

controller module

- [getButtonStateAndValue](#getButtonStateAndValue)
- [isButtonDown](#isButtonDown)
- [isButtonDown](#isButtonDown)
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

## isButtonDown

```lua
controller.isButtonDown(port, buttonId)
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

DpadUp = 1
DpadDown = 2
