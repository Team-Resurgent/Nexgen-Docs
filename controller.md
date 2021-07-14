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
Example: controller.Button['DpadDown']

| Input | Type | Description |
| --- | --- | --- |
| `DpadUp` | `string` | controller Dpad Up button Id = 1 |
| `DpadDown` | `string` | controller Dpad Down button Id = 2 |
| `DpadLeft` | `string` | controller Dpad Left button Id = 3 |
| `DpadRight` | `string` | controller Dpad Right button Id = 4 |
| `Start` | `string` | controller Start button Id = 5 |
| `Back` | `string` | controller Back button Id = 6 |
| `LeftThumb` | `string` | controller Left Thumb button Id = 7 |
| `RightThumb` | `string` | controller Right Thumb button Id = 8 |
| `LeftShoulder` | `string` | controller Left Shoulder button Id = 9 |
| `RightShoulder` | `string` | controller Right Shoulder button Id = 10 |
| `A` | `string` | controller A button Id = 11 |
| `B` | `string` | controller B button Id = 12 |
| `X` | `string` | controller X button Id = 13 |
| `Y` | `string` | controller Y button Id = 14 |
| `Black` | `string` | controller Black button Id = 15 |
| `White` | `string` | controller White button Id = 16 |
| `LeftTrigger` | `string` | controller Left Trigger button Id = 17 |
| `RightTrigger` | `string` | controller Right Trigger button Id = 18 |
| `LeftStickX` | `string` | controller Left Stick X analog stick Id = 19 |
| `LeftStickY` | `string` | controller Left Stick Y analog stick Id = 20 |
| `RightStickX` | `string` | controller Right Stick X analog stick Id = 21 |
| `RightStickY` | `string` | controller Right Stick Y analog stick Id = 22 |

