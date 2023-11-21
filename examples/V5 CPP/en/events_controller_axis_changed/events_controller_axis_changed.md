category: events  
signature: CONTROLLER.AXIS.changed(callback);  
device_class: controller  
description: Runs the specified function when the controller axis value changes.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Controller Axis Changed

Runs the specified function when the controller axis value changes.

```cpp
Controller1.Axis1.changed(callback);
```

## How To Use

Choose which Controller axis to monitor.

* `Axis1`
* `Axis2`
* `Axis3`
* `Axis4`

You will need to create a function to call when the Controller Axis position is changed. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Controller1.Axis1.changed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>