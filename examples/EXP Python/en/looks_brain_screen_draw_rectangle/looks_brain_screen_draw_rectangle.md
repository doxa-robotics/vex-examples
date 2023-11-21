category: looks  
signature: brain.screen.draw_rectangle(1, 1, 10, 10)  
description: Draws a rectangle on the EXP Brain's screen.  

# Draw Rectangle

Draws a rectangle on the EXP Brain's screen.

```don
brain.screen.draw_rectangle(X, Y, WIDTH, HEIGHT)
```

## How To Use

The `brain.screen.draw_rectangle()` command requires 4 values:

* Value 1: Top Left Corner X coordinate
* Value 2: Top Left Corner Y coordinate
* Value 3: Width of the rectangle
* Value 4: Height of the rectangle

The border line color of the rectangle is determined by the `brain.screen.set_pen_color()` command. The default line color is white.

The inside fill color of the rectangle is determine by the `brain.screen.set_fill_color()` command. The default fill color is black.

![brain_screen_info](exp_row_column_brain.jpg)

<advanced>
</advanced>
