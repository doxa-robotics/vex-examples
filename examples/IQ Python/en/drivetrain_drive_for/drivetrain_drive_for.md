category: drivetrain  
signature: drivetrain.drive_for(FORWARD, 2, MM, wait=True)  
description: Moves the Drivetrain in the specified direction for a given distance  

# Drive For

Moves the Drivetrain for a given distance. All Drivetrain motors run forward or in reverse at the velocity set by the Drivetrain's `Set Drive Velocity` command. After the Drivetrain has moved the specified distance the Drivetrain will stop.

```python
drivetrain.drive_for(DIRECTION, DISTANCE, UNITS)
```

## How To Use

Set how far the Drivetrain will move by entering at least three valid arguments inside of the parentheses, separated by commas. 

The first argument specifies the direction. Valid inputs are either `FORWARD` or `REVERSE` in all capital letters.  

The second argument specifies the distance that the IQ Robot should drive.

The third argument specifies the unit of measurement that should be used. Valid inputs are either `INCHES` or `MM` (millimeters) in all-capital letters.

The `DISTANCE` parameter accepts numeric values. Negative values will cause the IQ Robot to drive in the opposite of the input `DIRECTION`.

```python
drivetrain.drive_for(REVERSE, 5.0, INCHES)
```

The `Drive For` command is by default a blocking command. It will prevent subsequent commands from executing until the Drivetrain movement has completed.

## Optional Parameter

You can set a fourth parameter to `wait=False` to allow proceeding commands to run even before the Drivetrain is done moving.

```python
drivetrain.drive_for(FORWARD, 200, MM, wait=False)
```

## Example

This example shows the `Drive For` command being used with a variable as a distance.

The IQ Robot will drive 200 MM forward.

```python
distance_variable = 200
drivetrain.drive_for(FORWARD, distance_variable, MM)
```

<advanced>
</advanced>
