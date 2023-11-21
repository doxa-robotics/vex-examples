category: events  
signature: BUMPER.released(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Bumper Released

Runs the specified function when the bumper is released.

```cpp
BumperA.released(callback);
```

## How To Use

You will need to create a function to call when the Bumper Switch is released. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  BumperA.released(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```


<advanced>
</advanced>