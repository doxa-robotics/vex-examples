category: sensing  
signature: Drivetrain.isMoving()  
device_class: drivetrain  
description: Reports if the Drivetrain is currently moving.

# Drive Is Moving

Reports if the Drivetrain is currently moving.

```cpp
Drivetrain.isMoving()
```

## How To Use

This command returns **true** if the Drivetrain is moving because of a `Drivetrain.driveFor` or `Drivetrain.turnFor` command that specifies a set distance.

This command returns **false** if the Drivetrain movement has completed.

**Note:** This command will always return **false** if the Drivetrain is moving because of a `Drivetrain.drive` or `Drivetrain.turn` command (which do *not* specify a set distance to drive).

## Example

The example below prints whether the Drivetrain is moving to the VEX IQ brain's screen.

```cpp
Drivetrain.driveFor(forward, 1000, mm, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain is Moving: %s", Drivetrain.isMoving() ? "TRUE" : "FALSE");

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>