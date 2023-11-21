category: events  
signature: OPTICAL.objectLost(callback);  
device_class: optical  
description: Runs the callback function when a detected object is no longer being detected by a V5 Optical Sensor  

# Optical Object Lost

Runs the callback function when a detected object is no longer being detected by a V5 Optical Sensor.

```cpp
Optical.objectLost(callback);
```

## How To Use

The `Optical.objectLost();` command can be used to trigger actions or behaviors when a V5 Optical Sensor no longer detects a previously-detected object.

You will need to create a function to call when the object is no longer being detected. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```cpp
// Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Object lost!");
}

int main() {
  // Register event with a callback function
  Optical.objectLost(runOnEvent);
  
  while (true) {
    // Keep the main program running
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>







