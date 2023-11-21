category: sensing  
signature: GYRO.setRotation(90, degrees);  
device_class: gyro  
description: Sets the 3-Wire Gyro Sensor's angle of rotation to the value provided  

# Gyro Set Rotation

Sets the 3-Wire V5 Gyro Sensor's angle of rotation to the value provided.

```cpp
Gyro.setRotation(0, degrees);
```

## How To Use

The `Gyro.setRotation();` command can be used to set the Drivetrain's angle of rotation to any given positive (clockwise) or negative (counter-clockwise) value.

`Gyro.setRotation();` accepts any positive or negative decimal or integer number as a parameter.

```cpp
Gyro.setRotation(270, degrees);
Gyro.setRotation(-270, degrees);
```

<advanced>
</advanced>
