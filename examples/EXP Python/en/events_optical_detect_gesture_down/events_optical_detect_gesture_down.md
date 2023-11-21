category: events  
signature: optical.gesture_down(callback)   
device_class: optical  
description: Runs the callback function when the gesture is detected by an Optical Sensor  

# Optical Gesture Detected

Runs the callback function when gesture is detected by an Optical Sensor.

```python
optical.gesture_down(callback)
```

## How To Use

The `Optical Gesture Detected` command can be used to trigger actions or behaviors when a gesture is detected by an Optical Sensor.

You will need to create a function to call when a gesture is detected. Provide the name of the function that should run when the event occurs as the **callback** parameter.

You will also need to ensure that the Optical Sensor is set to detect gestures by calling `optical.gesture_enable()` before gesture commands are used.

`Optical Gesture Detected` can be used to detect four different gestures:

- `gesture_up`
- `gesture_down`
- `gesture_left`
- `gesture_right`

## Example

```python
# Function to run when the event occurs
def run_on_gesture_detected():
    brain.screen.print("Gesture detected!")

# Set the Optical Sensor to detect gestures
optical.gesture_enable()

# Register an event with a callback function
optical.gesture_down(run_on_gesture_detected)
```

<advanced>
</advanced>







