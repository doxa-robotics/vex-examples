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

```cpp
if (Drivetrain.isMoving()) {
  Brain.Screen.print("Moving!");
} else {
  Brain.Screen.print("Not Moving!");
}
```

<advanced>
</advanced>