category: looks  
signature: print("VEXcode")  
description: Prints values or text to the Print Console.  

# Console Print

Prints values or text to the Print Console.

```python
print("VEXcode")
```

## How To Use

The `print` command will print data at the cursor location on the Print Console.

All new projects begin with the cursor at row 1.

## Printing Lines

By default, Python will always add a new line after each `print` command.

To print multiple values to a single line, you can utilize the `end` parameter.

```python
print("This text will be ", end="")
print("printed on the same line")
```

## Printing Values

You can use the Python `format` method to format the values being printed in the print statements.

To use the `format` method, you must first provide a template string with replacement fields enclosed by a set of curly braces - `{}`.

Then, call the `format` method on the template string. Any parameter(s) passed into the `format` method will be inserted into the replacement fields in sequence (if there are multiple replacement fields).

You can also provide formatting options into the template string to set the number of decimal places to be printed. Any formatting options must begin with a semicolon - `:`.

In the example below, the value of the Brain Timer will be inserted into the single replacement field in the template string and printed to two decimal places.

```python
print("{:.2f}".format(brain.timer.time(SECONDS)))
```

Similarly, the example below will print the row/column position of the Brain Cursor. The number of replacement fields (enclosed by `{}`) must match the number of parameters passed into the `format` method.

```python
# The value of brain.screen.row() will be passed into the first replacement field
# The value of brain.screen.column() will be passed into the second replacement field
print("Row: {:d}, Column: {:d}".format(brain.screen.row(), brain.screen.column()))
```

Here is a list of commonly-used format specifiers. Remember that to use a format specifier inside a replacement field (enclosed by `{}`), it must follow a semicolon - `:`.

* `d` - Decimal Integer
* `f` - Floating Point Number
* `o` - Octal Integer
* `s` - String

Using the Floating Point Number format specifier, `f`, you can also specify how many decimal places to format a number.

* `.2f` - Formats a floating point number with 2 decimal places
* `.4f` - Formats a floating point number with 4 decimal places

## Printing Colors

You can use any of the color codes below with a `print` command to set the color of the text being printed.

The example below will show two ways in which a color sequence command can be used when printing. All color codes will need to be attached to an escape sequence - `\033`.

* `[31m` - Red
* `[32m` - Green
* `[34m` - Blue
* `[30m` - Black
* `[37m` - White
* `[33m` - Yellow
* `[91m` - Orange
* `[35m` - Purple
* `[36m` - Cyan
* `[97m` - Transparent

```python
# Using color codes in-line
# This will print "VEXcode" in Red to the Print Console
print("\033[31mVEXcode")

# Using color codes in separate commands
# Sets the print color for any subsequent prints
print("\033[31m")
print("VEXcode")
```

<advanced>
</advanced>
