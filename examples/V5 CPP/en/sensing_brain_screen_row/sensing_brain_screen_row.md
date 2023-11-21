category: sensing  
signature: Brain.Screen.row()  
description: Reports the row number of the V5 Brain screen cursor location.

# Brain Screen Row
Reports the row number of the V5 Brain screen cursor location.

```cpp
Brain.Screen.row()
```

## How To Use

`Brain.Screen.row()` reports an integer which ranges from **1 to 20**.

```cpp
if (Brain.Screen.row() > 10.0) {
  Brain.Screen.print("Cursor position is past row 10");
}
```
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