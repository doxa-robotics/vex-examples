category: sensing  
signature: optical.gesture_enable()  
description: Sets a V5 Optical Sensor to detect gestures  


# Optical Gesture Enable

Sets a V5 Optical Sensor to detect gestures.

```python
optical.gesture_enable()
```

## How To Use

The `Optical Gesture Enable` command allows you to set a V5 Optical Sensor to detect gestures.
 
By default, a V5 Optical Sensor will be set to detect colors.

Before using any V5 Optical Sensor gesture commands, a V5 Optical Sensor must be correctly set to detect gestures.

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