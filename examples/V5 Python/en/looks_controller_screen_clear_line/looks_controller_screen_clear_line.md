category: looks  
signature: controller.screen.clear_line()  
description: Clears a single row on the V5 Controller's screen.  

# Clear Row

Clears the current row on the V5 Controller's screen.

```don
controller.screen.clear_row()
```

Clears a specified row on the V5 Controller's screen.

```don
controller.screen.clear_row(ROW)
```

## How To Use

The `controller.screen.clear_row()` command can accept integer values between **1 - 3**, to set which row to clear. You can also call the command without any arguments to clear the current row.

---

The V5 Controller does not allow you to change the size of the font printed on the screen.

**V5 Controller Font Size - Number of Rows:**

* Standard Font - 3 Rows (Default)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
