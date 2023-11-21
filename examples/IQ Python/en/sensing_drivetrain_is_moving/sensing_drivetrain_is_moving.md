category: sensing  
signature: drivetrain.is_moving()
description: Reports if the Drivetrain is currently moving  

# Drive Is Moving
 
Reports if the Drivetrain is currently moving.

```python
drivetrain.is_moving()
```

## How To Use

`Drive Is Moving` reports **True** when the Drivetrain's motors are moving.

`Drive Is Moving` reports **False** when the Drivetrain's motors are stopped.

**Note:** This command will always return **false** if the Drivetrain is moving because of a `drivetrain.drive` or `drivetrain.turn` command (which do *not* specify a set distance to drive).

<advanced>
</advanced>
