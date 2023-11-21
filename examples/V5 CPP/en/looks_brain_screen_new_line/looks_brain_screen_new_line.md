category: looks  
signature: Brain.Screen.newLine();  
description: Sets the print output cursor on the V5 Brain's screen to the next available row.  

# Brain Screen New Line

Sets the print output cursor on the V5 Brain's screen to the next available row.

```cpp
Brain.Screen.newLine();
```

## How To Use

By default, all projects begin with the screen cursor at row 1 column 1. The `Brain.Screen.newLine();` command will move the cursor down by a single row on the screen. `Brain.Screen.newLine();` will also set the cursor's column to position 1.

---

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows available on the V5 Brain's screen.

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