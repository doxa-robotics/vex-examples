category: events  
signature: GPS.changed(callback);  
device_class: gps  
description: Runs the specified callback function when the GPS Sensor detects a heading change.  

# GPS When Heading Changed

Runs the specified callback function when the GPS Sensor detects a heading change.

```cpp
GPS.changed(callback);
```

## How To Use

You will need to define a function to call when the GPS Sensor detects a heading change.

Provide the name of the defined function that should run when the event occurs as the `callback` parameter.

```cpp
// Function to run when the event occurs
void runOnHeadingChange() {
  Brain.Screen.print("GPS Heading Change Detected");
}

int main() {
  // Register event with a callback function
  GPS.changed(runOnHeadingChange);

  while (true) {
    // Keep the main program running
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>