category: looks  
signature: Brain.Screen.clearLine();  
description: Clears a single row on the V5 Brain screen.  

# Brain Screen Clear Line
Clears the current row on the V5 Brain screen.

```cpp
Brain.Screen.clearLine();
```

Clears a specified row on the V5 Brain screen.

```cpp
Brain.Screen.clearLine(1);
```

## How To Use

The `Brain.Screen.clearLine();` command can accept integer values between **1 - 20**, to set which row to clear. You can also call the command without any arguments to clear the current row.

---

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of lines available on the V5 Brain's screen.

**V5 Brain Font Size - Number of Rows:**

* `mono12` - 20 Rows
* `mono15` - 16 Rows
* `mono20` / `prop20` - 12 Rows (Default)
* `mono30` / `prop30` - 8 Rows
* `mono40` / `prop40` - 6 Rows
* `mono60` / `prop60` - 4 Rows

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>