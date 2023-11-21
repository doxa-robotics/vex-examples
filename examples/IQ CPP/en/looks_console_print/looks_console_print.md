category: looks  
signature: printf("VEXcode");  
description: Prints values or text to the Print Console.  

# Console Print

Prints values or text to the Print Console

```cpp
printf("VEXcode");
```

## How To Use

The `printf` command will print data at the cursor location on the Print Console.

All new projects begin with the cursor at row 1.

The newline character, `\n` is needed in a `printf` command to output the contents of the Print Console buffer into the Print Console.

## Printing Values

You can use format specifiers to show values inside of your print statements:

* `%d` - Signed decimal integer
* `%f` - Decimal floating point number
* `%o` - Signed octal
* `%s` - String of characters
* `%x` - Unsigned hexadecimal integer
* `%c` - Character

```cpp
printf("Time Elapsed %f\n", Brain.Timer.value());
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
printf("Screen Pressed? %s\n", Brain.Screen.pressing());
```

## Printing Colors

You can use any of the color codes below with a `printf` command to set the color of the text being printed. The example below will show two ways in which a color sequence command can be used when printing. All color codes will need to be attached to an escape sequence - `\033`.

* `[31m` - Red
* `[32m` - Green
* `[34m` - Blue
* `[30m` - Black
* `[37m` - White
* `[33m` - Yellow
* `[91m` - Orange
* `[35m` - Purple
* `[38;5;207m` - Red Violet
* `[38;5;213m` - Violet
* `[38;5;063m` - Blue Violet
* `[38;5;081m` - Blue Green
* `[38;5;118m` - Yellow Green
* `[38;5;190m` - Yellow Orange
* `[38;5;214m` - Red Orange

```cpp
// Using color codes in-line
// This will print "VEXcode" in Red to the Print Console
printf("\033[31m VEXcode\n");

// Using color codes in separate commands
printf("\033[31m");
printf("VEXcode\n");
```

<advanced>
</advanced>