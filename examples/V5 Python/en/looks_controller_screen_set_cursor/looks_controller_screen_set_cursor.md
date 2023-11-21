category: looks  
signature: controller.screen.set_cursor(1, 1)  
description: Sets the cursor location for **controller.screen.print()** command on the V5 Controller's screen.

# Set Cursor


Sets the cursor location for **controller.screen.print()** command on the V5 Controller's screen.

```don
controller.screen.set_cursor(ROW, COLUMN)
```

## How To Use

The `controller.screen.set_cursor()` command requires 2 values:

* Value 1: Screen row position 
* Value 2: Screen column position

Set the cursor's row and column position to have a `controller.screen.print()` command display at a specific location on the screen.

`controller.screen.set_cursor()` accepts a range for **row** of **1 to 3**.

`controller.screen.set_cursor()` accepts a range for **column** of **1 to 20**.

---

The V5 Controller does not allow you to change the size of the font printed on the screen.

**V5 Controller Font Size - Number of Rows:**

* Standard Font - 3 Rows (Default)

**V5 Controller Font Size - Number of Columns:**

* Standard Font - 20 Columns (Default)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
