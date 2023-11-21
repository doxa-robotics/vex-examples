category: drive  
signature: Drivetrain.setDriveVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain that will be used for drive and driveFor calls. If this is used when the drive is moving, the drivetrain will be updated with the new speed. 

# Drivetrain Set Drive Velocity

Sets the velocity of the Drivetrain that will be used for `Drivetrain.drive` and `Drivetrain.driveFor` commands. 

If this command is used when the Drivetrain is moving, the Drivetrain movement will be updated with the new speed.

```cpp
Drivetrain.setDriveVelocity(velocity, units);
```

## How To Use

`Drivetrain.setDriveVelocity` will set the speed of the Drivetrain, but will not cause the Drivetrain to move by itself.

`Drivetrain.setDriveVelocity` accepts a range from **-100 to 100** when using **percent** units.

`Drivetrain.setDriveVelocity` accepts a range from **-127 to 127** when using **rpm** units.

Setting a Drivetrain's drive velocity to a negative value will cause the Drivetrain to drive in the opposite direction.

Setting a Drivetrain's drive velocity to 0 will prevent the Drivetrain from moving.

<advanced>
</advanced>