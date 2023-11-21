category: sensing  
signature: optical.get_gesture()  
description: Reports detected gesture data from a V5 Optical Sensor  


# Optical Gesture Detected

Reports detected gesture data from a V5 Optical Sensor.

```python
optical.get_gesture()
```

## How To Use

The `Optical Gesture Detected` command returns an object with gesture information. To check the type of the detected gesture, access the `type` property on the returned object.

```python
optical.get_gesture().type
```

Before using any V5 Optical Sensor gesture commands, a V5 Optical Sensor must be correctly set to detect gestures with the `optical.gesture_enable()` command.

Below are the gestures that a V5 Optical Sensor can detect:

- `GestureType.UP`
- `GestureType.DOWN`
- `GestureType.LEFT`
- `GestureType.RIGHT`

## Example

The example shows how to correctly set a V5 Optical Sensor to detect gestures before checking for gestures.

```python
optical.gesture_enable()
while optical.get_gesture().type != GestureType.UP:
    wait(0.1, SECONDS)
brain.screen.print("Up!")
```

<advanced>
</advanced>