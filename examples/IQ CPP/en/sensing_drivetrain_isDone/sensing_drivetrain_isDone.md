category: sensing  
signature: Drivetrain.isDone()  
device_class: drivetrain  
description: Reports if the Drivetrain has completed its movement.

# Drive Is Done

Reports if the Drivetrain has completed its movement.

```cpp
Drivetrain.isDone()
```

## How To Use

`Drivetrain.isDone` reports **true** when the Drivetrain's motors have completed their movement.

`Drivetrain.isDone` reports **false** when the Drivetrain's motors are still moving.

## Example

The example below prints whether the Drivetrain has completed its movements to the VEX IQ brain's screen.

```cpp
Drivetrain.driveFor(forward, 1000, mm, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain is Done: %s", Drivetrain.isDone() ? "TRUE" : "FALSE");

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>