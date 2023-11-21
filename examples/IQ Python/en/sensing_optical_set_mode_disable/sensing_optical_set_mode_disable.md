category: sensing  
signature: optical.gesture_disable()  
description: Sets an IQ Optical Sensor to detect colors  


# Optical Gesture Disable

Sets an IQ Optical Sensor to detect colors.

```python
optical.gesture_disable()
```

## How To Use

The `Optical Gesture Disable` command allows you to set an IQ Optical Sensor to detect colors.

By default, an IQ Optical Sensor will be set to detect colors.

## Example

The example shows how to correctly set an IQ Optical Sensor to detect colors after checking for gestures.

```python
# Detect gestures
optical.gesture_enable()
while optical.get_gesture().type != GestureType.UP:
    wait(0.1, SECONDS)
brain.screen.print("Up!")

wait(1, SECONDS)

# Detect colors
optical.gesture_disable()
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    if optical.color() == Color.RED:
        brain.screen.print("Red Object!")
    else:
        brain.screen.print("Not Red Object!")
    wait(0.02, SECONDS)

```

<advanced>
</advanced>