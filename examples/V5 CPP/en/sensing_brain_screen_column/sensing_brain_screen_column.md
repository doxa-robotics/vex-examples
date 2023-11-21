category: sensing  
signature: Brain.Screen.column()  
description: Reports the column number of the V5 Brain screen cursor location.

# Brain Screen Column
Reports the column number of the V5 Brain screen cursor location.

```cpp
Brain.Screen.column()
```

## How To Use

`Brain.Screen.column()` reports an integer which ranges from **1 to 80**.

```cpp
if (Brain.Screen.column() > 10.0) {
  Brain.Screen.print("Cursor is past column 10");
}
```
---

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of columns available on the V5 Brain's screen.

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