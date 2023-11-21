category: drivetrain
signature: drivetrain.set_timeout(TIME, SECONDS)
description: Sets a time limit for the Drivetrain's definite movement commands  

# Set Timeout

Sets a time limit for the Drivetrain's definite movement commands.

```python
drivetrain.set_timeout(TIME, SECONDS)
```

## How to Use

The command is used to prevent definite movement commands that do not reach their position from preventing other proceeding commands from running.

Specify the amount of time in `SECONDS`.

## Example

The example below sets the timeout of the Drivetrain to 3 seconds. If the Drivetrain does not complete its 2000 MM movement after 3 seconds has elapsed, it will stop driving.

```python
drivetrain.set_timeout(3, SECONDS)
drivetrain.drive_for(FORWARD, 2000, MM)
```

<advanced>
</advanced>
