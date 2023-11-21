category: sensing  
signature: drivetrain.is_done()
description: Reports if the Drivetrain has completed its movement.

# Drive Is Done

Reports if the Drivetrain has completed its movement.

```don
drivetrain.is_done()
```

## How To Use

Drive is done reports **True** when the robot's Drivetrain has completed its movement.

Drive is done reports **False** when the robot's Drivetrain is still moving.

**Note:** This command will always return **true** if the drivetrain is moving because of a `drive()` command.
	
<advanced>
</advanced>
