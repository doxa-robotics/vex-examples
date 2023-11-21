category: sensing  
signature: CONTROLLER.Screen.row()  
device_class: controller  
description: Reports the row number of the V5 Controller screen cursor location.

# Controller.Screen.row()

Reports the row number of the V5 Controller screen cursor location.

```cpp
Controller.Screen.row()
```

## How To Use

`Controller.Screen.row()` reports an integer which ranges from **1 to 3**.

```cpp
if (Controller1.Screen.row() > 2) {
}
```

---

Unlike V5 Brain, the V5 Controller does not allow you to change the size of the font printed on the screen. So there will always be 3 rows of spaces to print each row.

**V5 Controller Font Size - Number of Rows:**

* Standard Font - 3 Rows (Default)

![brain_screen_info_2](v5_controller_rows_columns.jpg)



<advanced>
</advanced>
<advanced>
</advanced>