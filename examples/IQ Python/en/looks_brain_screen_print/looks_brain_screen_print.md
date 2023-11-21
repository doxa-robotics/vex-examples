category: looks  
signature: brain.screen.print("VEXcode")  
description: Prints values or text on the IQ Brain's screen  

# Print

Prints values or text on the IQ Brain's screen.

```python
brain.screen.print("VEXcode")
```

## How To Use

The `Print` command will print data at a cursor location on the screen.

All new projects begin with the screen cursor at row 1 column 1.

* Print words and numbers: 
`brain.screen.print("Number:", 10)`

* Print the reported value from a variable: 
`brain.screen.print(my_variable)`

* Print the reported value from a sensor or device:  
`brain.screen.print(drivetrain.is_done())`

## Formatting Values

You can use either the `%` operator or the `format` function to adjust the precision of a printed value.

When displaying values, you can specify how many decimal places to print. For example, if your value is `3.14159265`, but you only want to display `3.14`, you can use either approach below to format it.

### Using the `%` Operator

The `%` operator can be used with any of the format specifiers listed below to format a floating point value.

A number before the decimal in the format specifier denotes the total number of characters to be printed.
If the value being printed is shorter than the total number of characters to be printed, the printed value is padded with blank spaces.

* `%d` - Prints a decimal integer
* `%f` - Prints a floating point number
* `%.2f` - Prints a floating point number to two decimal places
* `%6.2f` - Prints a floating point number with a minimum of six characters and two decimal places

Hence, to print `3.14` from `3.14159265`:

```python
brain.screen.print("%.2f" % 3.14159265)
```

### Using the `format` Function

The string `format` function can also be used to format a floating point value.

Similar to how the `%` operator is used, a format specifier denotes how a value will be formatted. However, the format string does not include the `%` operator, but utilizes `{}` to wrap a format specifier and calls the `format` function with a value to be formatted instead.

* `.d` - Prints a decimal integer
* `.f` - Prints a floating point number
* `.2f` - Prints a floating point number to two decimal places
* `6.2f` - Prints a floating point number with a minimum of six characters and two decimal places

Hence, to print `3.14` from `3.14159265`:

```python
brain.screen.print("{0:.2f}".format(3.14159265))
```

The `format` function can also be used to format and print more than one value. The value before the `:` (colon) in the format specifier is used to index a parameter from the `format` function call.

```python
brain.screen.print("{0:.2f}, {1:.2f}".format(1.234, 5.678))
```

In the above snippet, the `0` before the `:` in the first format specifier points to the first (zero-index) parameter in the `format` function call - `1.234`.

The `1` before the `:` in the second format specifier points to the second parameter in the `format` function call - `5.678`.

This will get printed to the IQ Brain:

```python
1.23, 5.68
```

<advanced>
</advanced>
