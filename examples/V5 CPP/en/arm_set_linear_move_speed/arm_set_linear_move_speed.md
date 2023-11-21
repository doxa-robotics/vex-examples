category: arm  
signature: RoboticArm.setLinearMoveSpeed(5.0);  
device_class: RoboticArm  
description: Sets the speed of the V5 Robotic Arm's linear movements.  

# Set linear speed

Sets the speed of the V5 Robotic Arm's linear movements.

```cpp
RoboticArm.setLinearMoveSpeed(5.0);
```

## How To Use

Specify the movement speed for linear movements in inches per second. The default speed is 5 inches per second. You can make the arm move faster by specifying a higher speed.

```cpp
RoboticArm.setLinearMoveSpeed(10.0);
```

You can make the arm move slower by specifiying a lower speed.

```cpp
RoboticArm.setLinearMoveSpeed(2.0);
```

<advanced>
</advanced>