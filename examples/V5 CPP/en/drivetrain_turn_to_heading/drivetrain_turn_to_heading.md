category: drive  
signature: Drivetrain.turnToHeading(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific heading, when using the Gyro or Inertial sensors.

# Drivetrain Turn To Heading

Turns a Drivetrain to a specific heading, when using the Gyro or Inertial sensors.

`Drivetrain.turnToHeading(heading, units);`

## How To Use

The `Drivetrain.turnToHeading();` command can be used to turn the Drivetrain to any given clockwise heading.

Based on the current heading of the Gyro, `Drivetrain.turnToHeading();` will determine which direction to turn.

`Drivetrain.turnToHeading();` accepts a range of **0.00 to 359.99** when using the unit `degrees`.

## Example

This example will cause the Drivetrain to make four turns: 

```cpp
Drivetrain.turnToHeading(45.0, degrees);
Drivetrain.turnToHeading(90.0, degrees);
Drivetrain.turnToHeading(270.0, degrees);
Drivetrain.turnToHeading(180.0, degrees);
```

- Right to 45 degrees
- Right to 90 degrees
- Right to 270 degrees
- Left to 180 degrees

The **turnToHeading** command will block other commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the **turnToHeading** command to not block the program until the movement has completed.

```cpp
Drivetrain.turnToHeading(180.0, degrees, false);
```

<advanced>
</advanced>