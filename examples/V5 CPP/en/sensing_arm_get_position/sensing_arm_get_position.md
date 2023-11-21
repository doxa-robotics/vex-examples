category: arm  
signature: RoboticArm.getAxisPosition(xaxis);  
device_class: RoboticArm  
description: Reports the current x, y, or z-coordinate position of the arm on the Workcell.

# Axis position

Reports the current x, y, or z-coordinate position of the arm on the Workcell.

```cpp
RoboticArm.getAxisPosition(xaxis);
```

## How To Use

The`RoboticArm.getAxisPosition(xaxis);` command is used to report the current x, y, or z-coordinate position of the arm on the Workcell.

Choose which axis to report. The arm of the Workcell operates in the x, y, and z-axes:

* **x-axis:** RoboticArm.getAxisPosition(xaxis);
* **y-axis:** RoboticArm.getAxisPosition(yaxis);
* **z-axis:** RoboticArm.getAxisPosition(zaxis);

<advanced>
</advanced>