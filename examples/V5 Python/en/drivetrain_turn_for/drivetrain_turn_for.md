category: drive  
signature: drivetrain.turn_for(RIGHT, 90, DEGREES, wait=True) 
description: Turns the Drivetrain for a given distance.  

# Turn For

Turns the Drivetrain for a specified number of degrees.

```don
drivetrain.turn_for(DIRECTION, ANGLE, UNITS)
```

## How To Use

The first argument specifies the turn direction: `LEFT` or `RIGHT`, written in all-capital letters. 

The second argument specifies the turn angle as a numeric value; this can be any number between 0 and 360. 

The third argument is the turn units. This should be set as `DEGREES` in all-capital letters. 

The `turn_for` command is by default a blocking command. It prevents any proceeding code from executing until the Drivetrain has completed its turn.

## Optional Parameters

If the fourth argument is set to `wait=False`, proceeding commands will be allowed to execute even before the Drivetrain has completed its turn.

```don
drivetrain.turn_for(LEFT, 90, DEGREES, wait=False)
```

## Example

This example will turn the V5 Robot 270 degrees to the right.

```don
drivetrain.turn_for(RIGHT, 270, DEGREES)
```

<advanced>
</advanced>
