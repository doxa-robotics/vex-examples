category: events  
signature: Brain.Timer.event(callback, 1000);  
description: Runs the specified function when the V5 Brain's timer is greater than the given value.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Brain Timer Event

Runs the specified callback function when the V5 Brain's timer is greater than the given value.

```cpp
Brain.Timer.event(callback, 1000);
```

## How To Use

The V5 Brain's timer begins at the beginning of each project.

Specify the amount of time. The `Brain.Timer.event();` event will run once the V5 Brain's timer is **greater than** the entered amount.

The `Brain.Timer.event();` command can accept integer values for the number of milliseconds.

You will need to create a function to call when the timer is greater than the entered amount. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Brain.Timer.event(runOnEvent, 2000);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```


<advanced>
</advanced>