category: sensing  
signature: Brain.Screen.yPosition()  
description: Reports the Y coordinate of the location of the last detected touch on the V5 Brain's touchscreen.

# Brain Screen yPosition
Reports the Y coordinate of the location of the last detected touch on the V5 Brain's touchscreen.

```cpp
Brain.Screen.yPosition()
```

## How To Use

`Brain.Screen.yPosition()` is used to capture the Y coordinate of the last press on the V5 Brain's touchscreen. 

It can be used with `Brain.Screen.xPosition()` to get the (x,y) coordinate, and create interactivity between the V5 and the end user.

`Brain.Screen.yPosition()` return an **integer** in a range of **0 to 240 pixels**.

![v5_row_column_brain](v5_row_column_brain.jpg)

```cpp
int myYCoordinate = Brain.Screen.yPosition();
```

<advanced>
</advanced>
