category: looks  
signature: CONTROLLER.Screen.newLine();  
device_class: controller  
description: Sets the print output cursor on the V5 Controller's screen to the next available row.  

# Controller Screen New Line

Sets the print output cursor on the V5 Controller's screen to the next available row.

```cpp
Controller.Screen.newLine();
```

## How To Use

By default, all projects begin with the screen cursor at row 1 column 1. The `Controller.Screen.newLine();` command will move the cursor down by a single row on the screen. `Controller.Screen.newLine();` will also set the cursor's column to position 1.

---

The V5 Controller does not allow you to change the size of the font printed on the screen.

**V5 Controller Font Size - Number of Rows:**

* Standard Font - 3 Rows (Default)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>