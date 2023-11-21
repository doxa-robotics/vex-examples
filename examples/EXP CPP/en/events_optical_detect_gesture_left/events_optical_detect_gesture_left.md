category: events  
signature: OPTICAL.gestureLeft(callback);  
device_class: optical  
description: Runs the callback function when the gesture is detected by an Optical Sensor  

# Optical Gesture Detected

Runs the callback function when the gesture is detected by an Optical Sensor.

```cpp
Optical.gestureLeft(callback);
```

## How To Use

The `Optical Gesture Detected` command can be used to trigger actions or behaviors when a gesture is detected by an Optical Sensor.

You will need to create a function to call when a gesture is detected. Provide the name of the function that should run when the event occurs as the **callback** parameter.

You will also need to ensure that the Optical Sensor is set to detect gestures by calling `Optical.gestureEnable();` before gesture commands are used.

`Optical Gesture Detected` can be used to detect four different gestures:

- `gestureUp`
- `gestureDown`
- `gestureLeft`
- `gestureRight`

## Example

```cpp
// Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Gesture detected!");
}

int main() {
  // Set the Optical Sensor to detect gestures
  Optical.gestureEnable();

  // Register event with a callback function
  Optical.gestureLeft(runOnEvent);
  
  while (true) {
    // Keep the main program running
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>







