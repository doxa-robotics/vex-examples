category: drive  
signature: drivetrain.drive(FOWARD)  
description: Moves the Drivetrain forever in the direction specified inside of the parentheses  

# Drive

Moves the Drivetrain forever in the direction specified inside the parentheses. 

All Drivetrain motors run forward or in reverse at the velocity set using the Drivetrain's `Set Drive Velocity` command. The default velocity is 50%.

Negative values will cause the Drivetrain to drive forward with a REVERSE input and in reverse with a FORWARD input.

```python
drivetrain.drive(DIRECTION)
```

## How To Use

The `Drive` command will run the Drivetrain forever, until a new drivetrain command is used, or the program is stopped.

## Examples

Use the `FORWARD` argument in all-capital letters to move the Drivetrain forward.

```python
drivetrain.drive(FORWARD)
```

Use the `REVERSE` argument in all-capital letters to move the Drivetrain in reverse.

```python
drivetrain.drive(REVERSE)
```
 
<advanced>
</advanced>
