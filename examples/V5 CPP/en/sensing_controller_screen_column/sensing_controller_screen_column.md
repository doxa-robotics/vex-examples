category: sensing  
signature: CONTROLLER.Screen.column()  
device_class: controller  
description: Reports the column number of the V5 Controller screen cursor location.

# Controller.Screen.column()

Reports the column number of the V5 Controller screen cursor location.

```cpp
Controller.Screen.column()
```

## How To Use

`Controller.Screen.column()` reports an integer which ranges from **1 to 19**.

```cpp
if (Controller1.Screen.column() > 10) {
}
```

---

Unlike V5 Brain, the V5 Controller does not allow you to change the size of the font printed on the screen. So there will always be 19 columns of spaces to print each row.

**V5 Controller Font Size - Number of Columns:**

* Standard Font - 19 Columns (Default)

![brain_screen_info_2](v5_controller_rows_columns.jpg)



<advanced>
</advanced>