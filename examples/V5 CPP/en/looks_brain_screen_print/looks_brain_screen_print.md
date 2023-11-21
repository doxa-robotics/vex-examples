category: looks  
signature: Brain.Screen.print("Hello");  
description: Prints values or text on the V5 Brain's screen.  

# Brain Screen Print

Prints values or text on the V5 Brain's screen.

```cpp
Brain.Screen.print("Hello World");
```

## How To Use

The `Brain.Screen.print();` command will print data at a cursor location on the screen.

All new projects begin with the screen cursor at row 1 column 1.

## Printing Values

You can use format specifiers to show values inside of your print statements:

* `%d` - Signed decimal integer
* `%f` - Decimal floating point number
* `%o` - Signed octal
* `%s` - String of characters
* `%x` - Unsigned hexadecimal integer
* `%c` - Character

```cpp
Brain.Screen.print("Time Elapsed %f", Brain.Timer.value());
```

When displaying values, you can specify how many decimals places to print. For example, if your value is `3.14159265`, but you only want to display `3.14`, your format specifier would be `%.2f`.

The number before the decimal in the format specifier denotes the total number of characters to be printed. If the value being printed is shorter than the total number of characters to be printed, the printed value is padded with blank spaces.

The format specifier can also contain flags, width, precision and modifiers sub-specifiers:

* `%d`	- Prints a decimal integer
* `%6d`	- Prints a decimal integer, with a minimum of 6 characters wide
* `%f`	- Prints a floating point number
* `%6f`	- Prints a floating point number, with a minimum of 6 characters wide
* `%.2f`  - Prints a floating point number, with 2 decimal characters places
* `%6.2f` - Prints a floating point number, with a minimum of 6 characters wide and 2 decimal places

```cpp
Brain.Screen.print("Time Elapsed %8.2f", Brain.Timer.value());
```

<advanced>
</advanced>