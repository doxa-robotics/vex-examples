category: sensing  
signature: GYRO.setHeading(90, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current position to the value provided. 

# Gyro Set Heading

Sets the Gyroscopic (Gyro) sensor's current position to the value provided. 

```cpp
Gyro.setHeading(0, degrees);
```

## How To Use

`Gyro.setHeading();` can be used to set the gyro's position to any clockwise heading. This command is typically used to reset the orientation of the gyro when the heading is set to a value of 0.

`Gyro.setHeading();` can accept decimals or integers.

```cpp
Gyro.setHeading(0, degrees);
```

<advanced>
</advanced>