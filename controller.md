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
controller.Button['buttonId']
```

Collection of button Id values to number

| Input | Type | Description |
| --- | --- | --- |
| `DpadUp` | `string` | controller Dpad Up button Id |
| `DpadDown` | `string` | controller Dpad Down button Id |
| `DpadLeft` | `string` | controller Dpad Left button Id |
| `DpadRight` | `string` | controller Dpad Right button Id |
| `Start` | `string` | controller Start button Id |
| `Back` | `string` | controller Back button Id |
| `LeftThumb` | `string` | controller Left Thumb button Id |
| `RightThumb` | `string` | controller Right Thumb button Id |
| `LeftShoulder` | `string` | controller Left Shoulder button Id |
| `RightShoulder` | `string` | controller Right Shoulder button Id |
| `A` | `string` | controller A button Id |
| `B` | `string` | controller B button Id |
| `X` | `string` | controller X button Id |
| `Y` | `string` | controller Y button Id |
| `Black` | `string` | controller Black button Id |
| `White` | `string` | controller White button Id |
| `LeftTrigger` | `string` | controller Left Trigger button Id |
| `RightTrigger` | `string` | controller Right Trigger button Id |
| `LeftStickX` | `string` | controller Left Stick X analog stick Id |
| `LeftStickY` | `string` | controller Left Stick Y analog stick Id |
| `RightStickX` | `string` | controller Right Stick X analog stick Id |
| `RightStickY` | `string` | controller Right Stick Y analog stick Id |

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
