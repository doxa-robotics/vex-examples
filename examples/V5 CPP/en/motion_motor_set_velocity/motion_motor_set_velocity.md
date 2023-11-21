category: motion  
signature: MOTOR.setVelocity(50, percent);  
device_class: motor  
description: Sets the V5 Motor or Motor Group's velocity.  

# Motor Set Velocity

Sets the V5 Smart Motor or or Motor Group's velocity.

```cpp
Motor.setVelocity(velocity, units);
```

## How To Use

`Motor.setVelocity();` will set the speed of the V5 Smart Motor or Motor Group but will not cause the Motor or Motor Group to move. 

`Motor.setVelocity();` accepts a range from **-100 to 100** when using the `percent` units.

`Motor.setVelocity();` accepts a range from **-600 to 600** when using the `rpm` units.

`Motor.setVelocity();` can use a "rotations per minute" (rpm) value based on the Gear Cartridge installed in the Motor or Motor Group.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

Setting a Motor or Motor Group's velocity to a negative value will cause the Motor/Motor Group to spin in the opposite direction.

Setting a Motor or Motor Group's velocity to 0 will cause the Motor/Motor Group to stop.

<advanced>
</advanced>