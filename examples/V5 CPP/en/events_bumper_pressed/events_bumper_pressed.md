category: events  
signature: BUMPER.pressed(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Bumper Pressed

Runs the specified function when the bumper is pressed.

```cpp
BumperA.pressed(callback);
```

## How To Use

You will need to create a function to call when the Bumper Sensor is pressed. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  BumperA.pressed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```



<advanced>
</advanced>