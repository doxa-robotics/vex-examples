category: arm  
signature: RoboticArm.setJointMoveSpeed(25.0);  
device_class: RoboticArm  
description: Sets the speed of the V5 Robotic Arm's joint movements.  

# Set joint speed

Sets the speed of the V5 Robotic Arm's joint movements.

```cpp
RoboticArm.setJointMoveSpeed(25.0);
```

## How To Use

Specify the movement speed for joint movements in degrees per second. The default speed is 25 degrees per second. You can make the arm move faster by specifying a higher speed.

```cpp
RoboticArm.setJointMoveSpeed(50.0);
```

You can make the arm move slower by specifiying a lower speed.

```cpp
RoboticArm.setJointMoveSpeed(10.0);
```

<advanced>
</advanced>