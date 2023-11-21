category: control  
signature: if condition:\n\tpass  
description: Used to decide whether or not a statement will be executed  

# If

A control statement used to decide whether a block of code will be executed based on the provided `condition`.

```don
if condition:
    pass
    
```

## How To Use

Replace the word `condition` with an expression that can either evaluate to `True` or `False`. An evaluation to `True` will allow the statement(s) indented below the `if` statement to execute.

Add a four-spaced indentation using the **spacebar** to include statements as part of the `if` control statement. 

An `if` statement should not contain an empty block of code. If necessary, add a `pass` statement to a previously empty `if` statement. 

## Example

This `if` statement will run if `my_variable` equals 1, causing the robot to drive forward.

```don
if my_variable == 1:
    drivetrain.drive(FORWARD)
```

<advanced>
</advanced>
