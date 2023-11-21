category: events  
signature: Brain.Screen.pressed(callback);  
description: Runs the callback function when the V5 Brain’s touchscreen is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Brain Screen Pressed

Runs the callback function when the V5 Brain’s touchscreen is pressed.

```cpp
Brain.Screen.pressed(callback);
```

## How To Use

The `Brain.Screen.pressed();` command can be used to trigger actions or behaviors based on touch interaction with the V5 Brain's touchscreen. 

Used together with the `Brain.Screen.xPosition()` and `Brain.Screen.yPosition()` commands, users can create custom interfaces to their V5 Brain by detecting when and where touches occur on the screen.

You will need to create a function to call when the screen gets pressed. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Brain.Screen.pressed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>