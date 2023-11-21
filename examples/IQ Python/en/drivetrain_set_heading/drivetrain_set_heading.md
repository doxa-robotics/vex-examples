category: drivetrain
signature: drivetrain.set_heading(0, DEGREES)  
description: Sets the Drivetrain's Inertial or Gyro Sensor to the specified heading    

# Set Heading

Sets the Drivetrain's Inertial or Gyro Sensor to the specified heading.

```python
drivetrain.set_heading(HEADING, DEGREES)
```

## How To Use

The Drivetrain's `Set Heading` command can be used to set the Drivetrain's heading to a specified value. This command can be used to reset the orientation of the Drivetrain's Inertial or Gyro Sensor when the heading is set to a value of 0.

`Set Heading` accepts a number value between **0 and 360** as it's first argument, and `DEGREES` written in all-capital letters as it's second argument.

## Example

This example sets the Drivetrain heading to 90 degrees. 

Since the heading of the IQ Robot is set to 90 degrees, the subsequent Drivetrain's `Turn to Heading` command will not cause the robot to turn as its current heading is already 90 degrees.

```python
drivetrain.set_heading(90, DEGREES)
drivetrain.turn_to_heading(90, DEGREES)
```

<advanced>
</advanced>
