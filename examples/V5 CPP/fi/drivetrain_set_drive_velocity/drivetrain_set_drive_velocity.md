category: drive  
signature: Drivetrain.setDriveVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain that will be used for drive and driveFor calls. If this is used when the drive is moving, the drivetrain will be updated with the new speed. 

# Drivetrain Set Drive Velocity

Sets the velocity of the Drivetrain that will be used for drive and driveFor calls. If this is used when the drive is moving, the drivetrain will be updated with the new speed.

```cpp
Drivetrain.setDriveVelocity(velocity, units);
```

## How To Use

`Drivetrain.setDriveVelocity();` will set the speed of the Drivetrain when driving straight, but will not cause the Drivetrain to move. 

`Drivetrain.setDriveVelocity();` accepts a range from **-100 to 100** when using the `percent` units.

`Drivetrain.setDriveVelocity();` accepts a range from **-600 to 600** when using the `rpm` units.

`Drivetrain.setDriveVelocity();` can use a "rotations per minute" (rpm) value based on the Gear Cartridge installed in the V5 Smart Motors used in the Drivetrain.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

Setting a Drivetrain's drive velocity to a negative value will cause the Drivetrain to drive in the opposite direction.

Setting a Drivetrain's drive velocity to 0 will cause the Drivetrain to stop.

<advanced>
</advanced>