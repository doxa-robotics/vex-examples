category: drive  
signature: drivetrain.drive(FOWARD)  
description: Moves the Drivetrain forever in the direction specified inside of the parentheses. 

# Drive

Moves the Drivetrain forever in the direction specified inside the parentheses. 

All drivetrain motors run forward or in reverse at the velocity set using the `drivetrain.set_drive_velocity` command. The default velocity is 50%. 

Negative values will cause the Drivetrain to drive forward with a REVERSE input and in reverse with a FORWARD input.

```don
drivetrain.drive(DIRECTION)
```

## How To Use

The `drivetrain.drive` command will run the Drivetrain forever, until a new drivetrain command is used, or the program is stopped.

## Examples

Use the `FORWARD` argument in all-capital letters to move the Drivetrain forward.

```don
drivetrain.drive(FORWARD)
```

Use the `REVERSE` argument in all-capital letters to move the Drivetrain in reverse.

```don
drivetrain.drive(REVERSE)
```
 
<advanced>
</advanced>
