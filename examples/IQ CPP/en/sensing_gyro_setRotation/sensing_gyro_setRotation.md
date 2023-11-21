category: sensing  
signature: Gyro.setRotation(rotation, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current rotation to the value provided. 

# Gyro Set Rotation

Sets the VEX IQ Gyro Sensor's angle of rotation to the specified rotation. 

```cpp
Gyro.setRotation(rotation, degrees);
```

## How To Use

The `Gyro.setRotation` command can be used to set the Drivetrain's angle of rotation to any given positive (counter-clockwise) or negative (clockwise) value.

`Gyro.setRotation` accepts a range of any positive or negative decimal or integer as the specified `rotation`.

## Example

The example below sets the rotation of the Gyro Sensor to -45 degrees.

```cpp
Gyro.setRotation(-45, degrees);
```

<advanced>
</advanced>