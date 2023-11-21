category: events  
signature: competition Competition = competition();
description: Create a new competition instance.

# New Competition

Create a new competition instance.

```cpp
competition Competition = competition();

competition Competition;
```

## How To Use

Using either of the above syntaxes, a new competition instance can be created before registering callback functions.

```cpp
// Create a new Competition instance
competition Competition;

// Function to run when the "autonomous" signal is received
void runOnAutonomous() {
  Brain.Screen.print("Running autonomous");
}

// Function to run when the "driver control" signal is received
void runOnDriverControl() {
  Brain.Screen.print("Running driver control");
}

int main() {
  // Register competition event with callback functions.
  Competition.autonomous(runOnAutonomous);
  Competition.drivercontrol(runOnDriverControl);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>