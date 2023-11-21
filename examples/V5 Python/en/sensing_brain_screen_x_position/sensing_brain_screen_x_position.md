category: sensing  
signature: brain.screen.x_position() 
description: Reports the X coordinate of the location of the last detected touch on the V5 Brain's touchscreen.

# Brain Screen xPosition
Reports the X coordinate of the location of the last detected touch on the V5 Brain's touchscreen.

```python
brain.screen.x_position()
```

## How To Use

`brain.screen.x_position()` is used to capture the X coordinate of the last press on the V5 Brain's touchscreen. 

It can be used with `brain.screen.y_position()` to get the (x,y) coordinate, and create interactivity between the V5 and the end user.

`brain.screen.x_position()` return an **integer** in a range of **0 to 480 pixels**.

![v5_row_column_brain](v5_row_column_brain.jpg)

```python
my_x_coordinate = brain.screen.x_position()
```


<advanced>
</advanced>
