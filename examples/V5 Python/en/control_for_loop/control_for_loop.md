category: control  
signature: for value in range (10): \n\tpass  
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# For

A type of loop that repeats the code contained in its body for a set number of iterations.

```don
for repeat_count in range(10):
    pass
```

# How To Use

First, replace `repeat_count` with a variable that will iterate through the `range()` function.

Second, replace `10` with a value to specify the end of the iteration.

Add a four-spaced indentation using the spacebar to include statements as part of the `for` control statement.

A `for` statement should not contain an empty block of code. If necessary, add a `pass` statement to a previously empty for statement.

Note that for loops start at the index 0 instead of 1.

`For` loops can also be nested inside each other.

# Example
The following for loop will print numbers 0 to 2:

```don
for i in range(3):
   brain.screen.print(i)
   brain.screen.new_line()
```
   
This will print:

```
0
1
2
```

<advanced>
</advanced>
