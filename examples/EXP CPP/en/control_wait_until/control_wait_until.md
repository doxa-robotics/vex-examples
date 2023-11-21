category: control  
signature: while (!condition) {\n\n};  
description: Waits for a condition to return true before moving to the next command.

# Wait Until

Repeats a segment of code until the provided **condition** returns **true**.

```cpp
while (!condition) { 
  // Code to repeat until condition returns true
}
```

## How To Use

This control statement will repeatedly check its condition, and will **not** execute any proceeding code until the condition returns **true**. At the same time, it will repeat any code provided between its curly braces.

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