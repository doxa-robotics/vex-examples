category: drivetrain 
signature: drivetrain.turn_to_heading(90, DEGREES)  
description: Turns a Drivetrain to a specific heading, when using the Gyro or Inertial sensors.

# Turn To Heading

Turns the Drivetrain to a specific heading when using the Gyro or Inertial sensors.

`drivetrain.turn_to_heading(HEADING, UNITS)`

## How To Use

The `drivetrain.turn_to_heading` command can be used to turn the Drivetrain to any given clockwise heading.

Based on the current Gyro heading, `drivetrain.turn_to_heading` will determine which direction to turn.

The `HEADING` parameter accepts numeric values in the range of **0.00 to 359.99** .

The `UNITS` parameter should be set to `DEGREES`.

## Example

This example will cause the Drivetrain to make four turns: 

```don
drivetrain.turn_to_heading(45.0, DEGREES)
drivetrain.turn_to_heading(90.0, DEGREES)
drivetrain.turn_to_heading(270.0, DEGREES)
drivetrain.turn_to_heading(180.0, DEGREES)
```

- Right to 45 degrees
- Right to 90 degrees
- Right to 270 degrees
- Left to 180 degrees

The `turn_to_heading` command will by default block proceeding commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `wait=False` as a third parameter to prevent the `turn_to_heading` command from blocking proceeding commands from executing until the Drivetrain turn has completed.

```don
drivetrain.turn_to_heading(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
