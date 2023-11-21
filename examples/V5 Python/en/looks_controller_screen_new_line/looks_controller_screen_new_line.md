category: looks  
signature: controller.screen.new_line()  
description: Sets the print output cursor on the V5 Controller's screen to the next available row.  

# Next Row

Sets the print output cursor on the V5 Controller's screen to the next available row.

```don
controller.screen.next_row()
```

## How To Use

By default, all projects begin with the screen cursor at row 1 column 1. The `controller.screen.next_row()` command will move the cursor down by a single row on the screen. `controller.screen.next_row()` will also set the cursor's column to position 1.

---

The V5 Controller does not allow you to change the size of the font printed on the screen.

**V5 Controller Font Size - Number of Rows:**

* Standard Font - 3 Rows (Default)

**V5 Controller Font Size - Number of Columns:**

* Standard Font - 20 Columns (Default)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
