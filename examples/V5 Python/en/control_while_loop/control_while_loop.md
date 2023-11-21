category: control  
signature: while expression: \n\tpass  
description: A loop that repeats the code while the condition returns true. 

# While
A loop that repeats the code in its body as long as the condition expression evaluates to **true**.   

```python
while condition:
    pass
```

## How To Use

The `while` loop will only check the condition inside the parenthesis at the beginning of each loop. 

If the condition evaluates to **true**, the code inside of `while` will run.

If the condition evaluates to **false**, the code inside of `while` will be skipped.

The `while` loop accepts anything that evaluates to `True` or `False` as its condition. You can place Booleans as well as expressions using comparison and logical operators. 

You can also use numerical values; **0** evaluates to `False`, and any **non-zero numbers** evaluates to `True`. 

Add a four-spaced indentation using the **spacebar** to include statements as part of the `while` control statement. 

A `while` statement should not contain an empty block of code. If necessary, add a `pass` statement to a previously empty `while` statement. 

## Example

This `while` loop will continue to print the word "Hello" on separate lines when the timer value is less than 50 seconds.

```python
while brain.timer.time(SECONDS) < 50:
    brain.screen.print("Hello")
    brain.screen.next_row()
```

<advanced>
</advanced>
