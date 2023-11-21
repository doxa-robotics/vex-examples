category: control  
signature: while (!condition) {\n\n};  
description: Waits for a condition to return true before moving to the next command.

# Wait Until

Run a set of commands until the **condition** evaluates to **true** before moving to the next command.

```cpp
while (!condition) {
  // Run some commands
}
```

## How To Use

The `while` loop will repeatedly check its condition, and will **not** execute any subsequent lines of code until the condition returns **true**.

```cpp
// Keep driving forward until the Bumper Pressing command returns true
while (!Bumper.pressing()) {
  Drivetrain.drive(forward);
}

// Stop the Drivetrain after the Bumper is pressed
Drivetrain.stop();
```

<advanced>
</advanced>