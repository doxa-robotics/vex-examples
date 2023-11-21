category: looks  
signature: Brain.Screen.setCursor(1, 1);  
description: Sets the cursor location for Brain.Screen.print(); command on the V5 Brain's screen.

# Brain Screen Set Cursor

Sets the cursor location for `Brain.Screen.print();` command on the V5 Brain's screen.

```cpp
Brain.Screen.setCursor(1, 2);
```

## How To Use

The `Brain.Screen.setCursor();` command requires 2 values:

* Value 1: Screen row position 
* Value 2: Screen column position

Set the cursor's row and column position to have a `Brain.Screen.print();` command display at a specific location on the screen.

Accepts a range for **row** of **1 to 20**.

Accepts a range for **column** of **1 to 80**.

---

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows and columns available on the V5 Brain's screen.

**V5 Brain Font Size - Number of Rows:**

* `mono12` - 20 Rows
* `mono15` - 16 Rows
* `mono20` / `prop20` - 12 Rows (Default)
* `mono30` / `prop30` - 8 Rows
* `mono40` / `prop40` - 6 Rows
* `mono60` / `prop60` - 4 Rows

**V5 Brain Font Size - Number of Columns:**

* `mono12` - 80 Columns
* `mono15` - 68 Columns
* `mono20` / `prop20` - 48 Columns (Default)
* `mono30` / `prop30` - 32 Columns
* `mono40` / `prop40` - 24 Columns
* `mono60` / `prop60` - 16 Columns

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>