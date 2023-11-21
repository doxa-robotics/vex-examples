category: drive  
signature: Drivetrain.setTimeout(1, seconds);  
device_class: drivetrain  
description: Sets the timeout for the Drivetrain to stop moving if a blocking command cannot reach its target.  

# Drivetrain Set Timeout

Sets the timeout for the Drivetrain to stop moving if a blocking command cannot reach its target.

```cpp
Drivetrain.setTimeout(time, seconds);
```

## How To Use

The `Drivetrain.setTimeout();` is used to prevent drive commands that do not reach their position from preventing other commands in the program from running.

An example of a Drivetrain not reaching its position is when a robot is driven against a wall and cannot complete its movement.

Set the timeout by specifying the amount of time in `seconds`.

```cpp
Drivetrain.setTimeout(2.0, seconds);
```

## Example

This example will end the `Drivetrain.driveFor();` command after 2 seconds if the Drivetrain has not reached the target of 24 inches. 

Once the time limit or distance is reached, the Drivetrain will move on to the `Drivetrain.turnFor();` command.

```cpp
Drivetrain.setTimeout(2.0, seconds);
Drivetrain.driveFor(24.0, inches, true);
Drivetrain.turnFor(90.0, degrees, true);
```

<advanced>
</advanced>