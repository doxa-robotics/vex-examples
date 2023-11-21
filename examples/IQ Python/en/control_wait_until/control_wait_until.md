category: control  
signature: while not expression: \n\tpass  
description: A loop that continues until the expression turns true.  

# While Not
A control statement that continues looping until the expression turns **True**.

```python
while not condition:
    pass
```

## How To Use

The `while not` statement will repeatedly check the condition, and will not move to the next command until the condition reports **True**.

If the condition evaluates to **False**, the code inside of `while not` will run.

If the condition evaluates to **True**, the code inside of `while not` will be skipped, and the next command after the `while not` statement will be executed.

The `while not` statement accepts any expression that evaluates to `True` or `False` as its condition. You can place Booleans as well as expressions using comparison and logical operators. 

You can also use numerical values; **0** evaluates to `False`, and any **non-zero numbers** evaluates to `True`. 

Add a four-spaced indentation using the **spacebar** to include statements as part of the `while not` control statement. 

A `while not` statement should not contain an empty block of code. If necessary, add a `pass` statement to a previously empty `while not` statement. 

Add a brief delay after each loop iteration for optimal loop performance (see example below).

## Example

This `while not` loop will print "Hello" on separate lines until the value of my_variable is equal to 5.

```python
my_variable = 0

while not my_variable == 5:
    brain.screen.print("Hello")
    brain.screen.new_line()
    my_variable += 1
    wait(0.1, SECONDS)
```

<advanced>
</advanced>
