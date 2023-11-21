category: drivetrain 
signature: drivetrain.drive_for(FORWARD, 2, MM, wait=True)
description: Moves the Drivetrain for a given distance.  

# Drive For

Moves the Drivetrain for a given distance. All drivetrain motors run forward or in reverse at the velocity set by the `drivetrain.set_drive_velocity` command. After the Drivetrain has moved the input distance the Drivetrain will stop.

```don
drivetrain.drive_for(DIRECTION, DISTANCE, UNITS)
```

## How To Use

Set how far the Drivetrain will move by entering at least three valid arguments inside of the parentheses, separated by commas. 

The first argument specifies the direction. Valid inputs are either `FORWARD` or `REVERSE` in all capital letters.  

The second argument specifies the distance that the V5 Robot should drive.

The third argument specifies the unit of measurement that should be used. Valid inputs are either `INCHES` or `MM` (millimeters) in all-capital letters.

The `DISTANCE` parameter accepts numeric values. Negative values will cause the V5 Robot to drive in the opposite of the input `DIRECTION`.

```
drivetrain.drive_for(REVERSE, 5.0, INCHES)
```

The `drive_for` command is by default a blocking command. It will prevent subsequent commands from executing until the Drivetrain movement has completed.

## Optional Parameter

You can set a fourth parameter to `wait=False` to allow proceeding commands to run even before the Drivetrain is done moving.

```don
drivetrain.drive_for(FORWARD, 200, MM, wait=False)
```

## Example

This example shows the `drivetrain.drive_for` being used with a variable as a distance.

The V5 Robot will drive 200 MM forward.

```don
distance_variable = 200

drivetrain.drive_for(FORWARD, distance_variable, MM)
```

<advanced>
</advanced>
