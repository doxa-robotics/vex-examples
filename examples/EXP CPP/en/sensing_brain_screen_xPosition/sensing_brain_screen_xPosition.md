category: sensing  
signature: Brain.Screen.xPosition()  
description: Reports the X coordinate of the location of the last detected touch on the EXP Brain's touchscreen.

# Brain Screen xPosition
Reports the X coordinate of the location of the last detected touch on the EXP Brain's touchscreen.

```cpp
Brain.Screen.xPosition()
```

## How To Use

`Brain.Screen.xPosition()` is used to capture the X coordinate of the last press on the EXP Brain's touchscreen. 

It can be used with `Brain.Screen.yPosition()` to get the (x,y) coordinate, and create interactivity between the EXP Brain and the end user.

`Brain.Screen.xPosition()` return an **integer** in a range of **0 to 160 pixels**.

![row_column_brain](exp_row_column_brain.jpg)

```cpp
int myXCoordinate = Brain.Screen.xPosition();
```


<advanced>
</advanced>
