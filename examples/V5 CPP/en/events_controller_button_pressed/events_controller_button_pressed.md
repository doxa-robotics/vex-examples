category: events  
signature: CONTROLLER.BUTTON.pressed(callback);  
device_class: controller  
description: Runs the specified function when the controller button is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Controller Button Pressed

Runs the specified function when the controller button is pressed.

```cpp
Controller1.ButtonA.pressed(callback);
```

## How To Use

Choose which Controller button to monitor.

* `ButtonA`
* `ButtonB`
* `ButtonX`
* `ButtonY`
* `ButtonUp`
* `ButtonDown`
* `ButtonLeft`
* `ButtonRight`
* `ButtonL1`
* `ButtonL2`
* `ButtonR1`
* `ButtonR2`

You will need to create a function to call when the Controller Button is pressed. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Controller1.ButtonA.pressed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```



<advanced>
</advanced>