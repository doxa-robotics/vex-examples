category: drivetrain 
signature: drivetrain.turn_to_heading(90, DEGREES)  
description: Turns a Drivetrain to a specific heading, when using a Gyro or Inertial Sensor  

# Turn To Heading

Turns a Drivetrain to a specific heading, when using a Gyro or Inertial Sensor.

```python
drivetrain.turn_to_heading(HEADING, DEGREES)
```

## How To Use

The `Turn to Heading` command can be used to turn the Drivetrain to any given clockwise or counter-clockwise positive heading, depending on whether a Gyro or Inertial Sensor is configured with the Drivetrain.

Based on the current heading, `Turn to Heading` will determine the shortest direction to turn.

The `HEADING` parameter accepts numeric values in the range of **0.00 to 359.99** .

The second parameter should be set to `DEGREES`.

## Example

This example will cause the Drivetrain to make four turns:

```python
drivetrain.turn_to_heading(45.0, DEGREES)
drivetrain.turn_to_heading(90.0, DEGREES)
drivetrain.turn_to_heading(270.0, DEGREES)
drivetrain.turn_to_heading(180.0, DEGREES)
```

- Right to 45 degrees
- Right to 90 degrees
- Right to 270 degrees
- Left to 180 degrees

(The direction descriptions below are based on a clockwise positive heading, with the IQ (2nd generation) Brain's Inertial Sensor configured with the Drivetrain)

The `Turn to Heading` command will by default block proceeding commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `wait=False` as a third parameter to prevent the `Turn to Heading` command from blocking proceeding commands from executing until the Drivetrain turn has completed.

```python
drivetrain.turn_to_heading(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
