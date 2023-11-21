category: drive  
signature: Drivetrain.setTurnVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain when turning. If this is used when the drivetrain is turning, the drivetrain will be updated with the new speed.  

# Drivetrain Set Turn Velocity

Sets the velocity of the Drivetrain when turning. If this is used when the drivetrain is turning, the drivetrain will be updated with the new speed.

```cpp
Drivetrain.setTurnVelocity(velocity, units);
```

## How To Use

`Drivetrain.setTurnVelocity();` will set the speed of the Drivetrain when turning, but will not cause the Drivetrain to move. 

`Drivetrain.setTurnVelocity();` accepts a range from **-100 to 100** when using the `percent` units.

`Drivetrain.setTurnVelocity();` accepts a range from **-600 to 600** when using the `rpm` units.

`Drivetrain.setTurnVelocity();` can use a "rotations per minute" (rpm) value based on the Gear Cartridge installed in the V5 Smart Motors used in the Drivetrain.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

Setting a Drivetrain's turn velocity to a negative value will cause the Drivetrain to turn in the opposite direction.

Setting a Drivetrain's turn velocity to 0 will cause the Drivetrain to stop.

<advanced>
</advanced>