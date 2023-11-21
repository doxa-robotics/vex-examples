category: functions  
signature: def function_name(parameters):\n\tpass  
description: Functions are blocks of code used to perform an action.

# Functions

Functions are blocks of code used to perform an action.

## How To Use

To create a function, create a meaningful function name. This means that the function name should accurately describe what it does.

Use the **keyword** `def` before your function name to define the function.

Include parentheses `()` enclosing optional parameters after the function name, followed by a colon`:`. Multiple parameters should be separated by commas `(parameter1, parameter2)`.

The body of the function should be indented four spaces. If there isn't any code for the function to execute, a `pass` should be included in the function definition.

```don
def my_function():
    pass
```

## Example 1

This function has no parameters and will print "Hello" to the EXP Brain Screen.

```don
def print_hello_world():
    brain.screen.print("Hello World")
```
## Example 2

This function takes one parameter, `name` and will print the value of `name` to the EXP Brain Screen.

```don
def print_name(name):
    brain.screen.print(name)
```

<advanced>
</advanced>
