category: looks  
signature: brain.screen.set_cursor(1, 1)
description: Sets the cursor location for brain.screen.print() command on the V5 Brain's screen.

# Set Cursor


Sets the cursor location on the V5 Brain's screen.

```don
brain.screen.set_cursor(ROW, COLUMN)
```

## How To Use

The `brain.screen.set_cursor()` command requires 2 values:

* Value 1: Screen row position 
* Value 2: Screen column position

Set the cursor's row and column position to have a `brain.screen.print()` command display at a specific location on the screen.

Accepts a range for **row** of **1 to 20**.

Accepts a range for **column** of **1 to 80**.

---

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows and columns available on the V5 Brain's screen.

**V5 Brain Font Size - Number of Rows:**

* `FontType.MONO12` - 20 Rows
* `FontType.MONO15` - 16 Rows
* `FontType.MONO20` / `FontType.PROP20` - 12 Rows (Default)
* `FontType.MONO30` / `FontType.PROP30` - 8 Rows
* `FontType.MONO40` / `FontType.PROP40` - 6 Rows
* `FontType.MONO60` / `FontType.PROP60` - 4 Rows

**V5 Brain Font Size - Number of Columns:**

* `FontType.MONO12` - 80 Columns
* `FontType.MONO15` - 68 Columns
* `FontType.MONO20` / `FontType.PROP20` - 48 Columns (Default)
* `FontType.MONO30` / `FontType.PROP30` - 32 Columns
* `FontType.MONO40` / `FontType.PROP40` - 24 Columns
* `FontType.MONO60` / `FontType.MONO60` - 16 Columns

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
