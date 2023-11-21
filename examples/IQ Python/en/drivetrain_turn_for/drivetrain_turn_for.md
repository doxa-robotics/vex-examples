category: drive  
signature: drivetrain.turn_for(RIGHT, 90, DEGREES, wait=True) 
description: Turns the Drivetrain in the specified direction for a set number of degrees  

# Turn For

Turns the Drivetrain in the specified direction for a set number of degrees.

```python
drivetrain.turn_for(DIRECTION, ANGLE, DEGREES)
```

## How To Use

The first argument specifies the turn direction: `LEFT` or `RIGHT`, written in all-capital letters. 

The second argument specifies the turn angle as a numeric value; this can be any number or numeric variable. 

The third argument is the turn units. This should be set as `DEGREES` in all-capital letters. 

The `Turn For` command is by default a blocking command. It prevents any proceeding code from executing until the Drivetrain has completed its turn.

## Optional Parameters

If the fourth argument is set to `wait=False`, proceeding commands will be allowed to execute even before the Drivetrain has completed its turn.

```python
drivetrain.turn_for(LEFT, 90, DEGREES, wait=False)
```

## Example

This example will turn the IQ Robot 270 degrees to the right.

```python
drivetrain.turn_for(RIGHT, 270, DEGREES)
```

<advanced>
</advanced>
