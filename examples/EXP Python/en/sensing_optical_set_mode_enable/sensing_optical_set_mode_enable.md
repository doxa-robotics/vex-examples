category: sensing  
signature: optical.gesture_enable()  
description: Sets an Optical Sensor to detect gestures  


# Optical Gesture Enable

Sets an Optical Sensor to detect gestures.

```python
optical.gesture_enable()
```

## How To Use

The `Optical Gesture Enable` command allows you to set an Optical Sensor to detect gestures.
 
By default, an Optical Sensor will be set to detect colors.

Before using any Optical Sensor gesture commands, an Optical Sensor must be correctly set to detect gestures.

## Example

The example shows how to correctly set an Optical Sensor to detect gestures before checking for gestures.

```python
optical.gesture_enable()
while optical.get_gesture().type != GestureType.UP:
    wait(0.1, SECONDS)
brain.screen.print("Up!")
```

<advanced>
</advanced>