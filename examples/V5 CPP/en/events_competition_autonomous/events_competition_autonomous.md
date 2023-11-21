category: events  
signature: Competition.autonomous(callback);  
description: Runs the specified function when an "autonomous" mode signal is received from a competition field or competition switch.<br /><br />A competition object must be defined, or the program must be a competition template.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Competition Autonomous

Runs the specified function when an "autonomous" mode signal is received from a competition field or competition switch.

Make sure that the competition object is defined or use a competition template from the Examples Projects.

```cpp
Competition.autonomous(callback);
```

## How To Use

You will need to create a function to call when the Competition Autonomous signal is received. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Create a Competition Object
competition Competition;

//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Competition.autonomous(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>