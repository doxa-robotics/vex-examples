category: sensing  
signature: Drivetrain.isMoving()  
device_class: drivetrain  
description: Reports if the Drivetrain is currently moving.

# Drivetrain Is Moving

Reports if the Drivetrain is currently moving.

```cpp
Drivetrain.isMoving()
```

## How To Use

This command returns **true** if the drivetrain is moving because of a `driveFor()` or `turnFor()` command that *does* specify a set distance.

This command returns **false** if the drivetrain movement has completed.

**Note:** This command will always return **false** if the drivetrain is moving because of a `drive()` or `turn()` command that does *not* specify a set distance.

## Example

The example below prints whether the Drivetrain is moving to the EXP brain's screen.

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