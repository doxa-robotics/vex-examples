category: sensing  
signature: INERTIAL.setRotation(90, degrees);  
device_class: inertial  
description: Sets the V5 Inertial Sensor's angle of rotation to the value provided  

# Inertial Set Rotation

Sets the V5 Inertial Sensor's angle of rotation to the value provided.

```cpp
Inertial.setRotation(0, degrees);
```

## How To Use

The `Inertial.setRotation()` command can be used to set the Drivetrain's angle of rotation to any given positive (clockwise) or negative (counter-clockwise) value.

`Inertial.setRotation()` accepts any positive or negative decimal or integer number.

```cpp
Inertial20.setRotation(0, degrees)
```

<advanced>
</advanced>
