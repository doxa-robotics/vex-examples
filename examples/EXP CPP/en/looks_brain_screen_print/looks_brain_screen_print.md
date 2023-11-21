category: looks  
signature: Brain.Screen.print("Hello");  
description: Prints values or text on the EXP Brain's screen.  

# Brain Screen Print

Prints values or text on the VEX EXP Brain's screen.

```cpp
Brain.Screen.print();
```

## How To Use

The `Brain.Screen.print` command will print data at a cursor location on the screen.

All new projects begin with the screen cursor at row 1 column 1.

Print string values:

```cpp
Brain.Screen.print("String: 123 + Words");
```

Print integer or decimal values:

```cpp
// When printing integer values, the "%d" format specifier is
// required as the first parameter

Brain.Screen.print("Integer: %d", 5 + 10);

// When printing decimal values, the "%f" format specifier is
// required as the first parameter

Brain.Screen.print("Decimal: %f", 5.0 + 10.0);
```

Print the reported value from a sensing command:

```cpp
// If the reported value is a decimal or integer,
// use "%f" or "%d" respectively as the format specifier

Brain.Screen.print("%d", Brain.Timer.time());

// If the reported value is a boolean,
// use "%s" as the format specifier

Brain.Screen.print("%s", Motor.isDone() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>