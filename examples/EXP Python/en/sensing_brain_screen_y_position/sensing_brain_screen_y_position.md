category: sensing  
signature: brain.screen.y_position()
description: Reports the Y coordinate of the location of the last detected touch on the EXP Brain's touchscreen.

# Brain Screen yPosition
Reports the Y coordinate of the location of the last detected touch on the EXP Brain's touchscreen.

```python
brain.screen.y_position()
```

## How To Use

`brain.screen.y_position()` is used to capture the Y coordinate of the last press on the EXP Brain's touchscreen. 

It can be used with `brain.screen.x_position()` to get the (x,y) coordinate, and create interactivity between the EXP and the end user.

`brain.screen.y_position()` return an **integer** in a range of **0 to 240 pixels**.

![exp_row_column_brain](exp_row_column_brain.jpg)

```python
my_y_coordinate = brain.screen.y_position()
```

<advanced>
</advanced>
