category: sensing  
signature: INERTIAL.setHeading(0, degrees);  
device_class: inertial  
description: Sets the Inertial sensor's current heading position to a set value.

# Inertial Set Heading

Sets the Inertial sensor's current heading position to a set value.

```cpp
Inertial.setHeading(0, degrees);
```

## How To Use

`Inertial.setHeading()` can be used to set the Gyro's position to any clockwise heading. This command is typically used to reset the orientation of the Inertial Sensor when the heading is set to a value of 0.

`Inertial.setHeading()` accepts a range of **0.0 to 359.99** degrees.

`Inertial.setHeading()` can accept decimals, integers, or other commands that return a numeric value.


```cpp
myInertial.setHeading(0, degrees);
```

<advanced>
</advanced>
