category: looks  
signature: Brain.Screen.clearLine();  
description: Clears a single row on the Brain screen.  

# Clear Line

Clears the current row on the VEX IQ Brain's Screen.

```cpp
Brain.Screen.clearLine();
```

Clears a specified row on the Brain's screen.

```cpp
Brain.Screen.clearLine(1);
```

## How To Use

You can call the `Brain.Screen.clearLine` command without any arguments to clear the current row.

### IQ (1st generation) Brain

The `Brain.Screen.clearLine` command can accept integer values between **1 to 5**, to set which row to clear. 

![row_column_index](row_column_index.png)

### IQ (2nd generation) Brain

The IQ (2nd generation) Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows and columns available on the Brain's screen.

| Font |  | Rows |  | Columns |
| :--- | --- | :--- | --- | :--- |
| Mono Extra Small (mono12) |  | 9 |  | 26 |
| Mono Small (mono15) |  | 7 |  | 20 |
| Mono Medium (mono20) (Default) |  | 5 |  | 16 |
| Mono Large (mono30) |  | 3 |  | 10 |
| Mono Extra Large (mono40) |  | 3 |  | 8 |
| Mono Super Large (mono60) |  | 1 |  | 5 |
| Prop Medium (prop20) |  | 5 |  | 28 |
| Prop Large (prop30) |  | 3 |  | 21 |
| Prop Extra Large (prop40) |  | 2 |  | 15 |
| Prop Super Large (prop60) |  | 1 |  | 9 |

`Brain.Screen.clearLine` accepts a range of values from **1 to 9** for the row to clear, depending on what font is currently selected.

![row_column_index2](iq2_row_column_brain2.jpg) 

## Example 
This example will print "Hello" on row 2, column 1, wait for three seconds, then clear row 2.

```cpp
Brain.Screen.setCursor(2, 1);
Brain.Screen.print("Hello");
wait(3.0, seconds);
Brain.Screen.clearLine(2);
```

<advanced>
</advanced>