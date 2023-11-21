category: events  
signature: OPTICAL.objectDetected(callback);  
device_class: optical  
description: Runs the callback function when an object is detected by an Optical Sensor  

# Optical Object Detected


Runs the callback function when an object is detected by an Optical Sensor.

```cpp
Optical.objectDetected(callback);
```

## How To Use

The `Optical.objectDetected();` command can be used to trigger actions or behaviors when an object is detected by an Optical Sensor.

You will need to create a function to call when an object is detected. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```cpp
// Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Object detected!");
}

int main() {
  // Register event with a callback function
  Optical.objectDetected(runOnEvent);
  
  while (true) {
    // Keep the main program running
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>







