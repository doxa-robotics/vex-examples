category: control  
signature: if condition: \n\tpass\nelse:\n\tpass  
description: Used to decide if one statement will execute or another will if the first statement is not true.

# If/else
A control flow statement that executes one block of commands if a condition evaluates to true, or another block of commands if a condition evaluates to false. 

```don
if condition:
    pass
else:
    pass

```

## How To Use

The `if` statement is a conditional that will check if its condition evaluates to **True** or **False**. It is possible to combine many conditions with the use of logical operators such as `and`, `or`, and `not`. 

If the totality of the condition is **True**, then the code block indented below the `if condition:` will run. If the totality of the condition is **False**, the code block indented below the `else:` statement will run instead.

Code blocks below the `if` and `else` should be indented four spaces.

An `if/else` statement should not contain empty blocks of code. If necessary, add  `pass` statements to a previously empty `if/else` statement. 

## Example

This `if/else` code will drive the robot FORWARD if the variable equals 1. If it does not, it will drive the robot REVERSE. 

```don
if my_variable == 1:
    drivetrain.drive(FORWARD)
else:
    drivetrain.drive(REVERSE)
```

<advanced>
</advanced>
