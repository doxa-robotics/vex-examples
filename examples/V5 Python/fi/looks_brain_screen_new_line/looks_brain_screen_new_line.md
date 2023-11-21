category: looks  
signature: brain.screen.new_line()  
description: Sets the print output cursor on the V5 Brain's screen to the next available row.  

# Next Row

Sets the print output cursor on the V5 Brain's screen to the next available row.

```don
brain.screen.next_row()
```

## How To Use

By default, all projects begin with the screen cursor at row 1 column 1. The `brain.screen.next_row()` command will move the cursor down by a single row on the screen. `brain.screen.next_row()` will also set the cursor's column to position 1.

---

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows available on the V5 Brain's screen.

**V5 Brain Font Size - Number of Rows:**

* `FontType.MONO12` - 20 Rows
* `FontType.MONO15` - 16 Rows
* `FontType.MONO20` / `FontType.PROP20` - 12 Rows (Default)
* `FontType.MONO30` / `FontType.PROP30` - 8 Rows
* `FontType.MONO40` / `FontType.PROP40` - 6 Rows
* `FontType.MONO60` / `FontType.PROP60` - 4 Rows

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
