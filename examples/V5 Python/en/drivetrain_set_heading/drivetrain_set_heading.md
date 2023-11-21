category: drivetrain
signature: drivetrain.set_heading(0, DEGREES)  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Set Heading

Sets the Gyro of the Drivetrain to an exact heading.

```don
drivetrain.set_heading(HEADING, UNITS)
```

## How To Use

The `drivetrain.set_heading` command can be used to set the Drivetrain's position to any given heading. This command can be used to reset the orientation of the Drivetrain's Gyro when the heading is set to a value of 0.

`drivetrain.set_heading` accepts a number value between **0 and 360** as it's first argument, and `DEGREES` written in all-capital letters as it's second argument.

## Example

This example sets the Drivetrain heading to 90 degrees. 

Since the heading of the V5 Robot is set to 90 degrees, the subsequent `turn_to_heading` command will not cause the robot to turn as its current heading has already been set to 90 degrees.

```don
drivetrain.set_heading(90, DEGREES)
drivetrain.turn_to_heading(90, DEGREES)
```

<advanced>
</advanced>
