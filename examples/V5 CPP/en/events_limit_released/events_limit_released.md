category: events  
signature: LIMIT.released(callback);  
device_class: limit  
description: Runs the specified function when the Limit Switch is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# LimitSwitch Released

Runs the specified function when the Limit Switch is released.

```cpp
LimitA.released(callback);
```

## How To Use

You will need to create a function to call when the Limit Switch is released. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  LimitA.released(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```


<advanced>
</advanced>