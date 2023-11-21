category: sensing  
signature: drivetrain.is_moving()
description: Reports if the Drivetrain is currently moving.

# Drive Is Moving
 
Reports if the Drivetrain is currently moving.

```don
drivetrain.is_moving()
```

## How To Use

Drive is moving reports **True** when the Drivetrain's motors are moving.

Drive is moving reports **False** when the Drivetrain's motors are stopped.

**Note:** This command will always return **false** if the drivetrain is moving because of a `drive()` command.

<advanced>
</advanced>
