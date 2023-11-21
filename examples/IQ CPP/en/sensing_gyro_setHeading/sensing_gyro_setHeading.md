category: sensing  
signature: Gyro.setHeading(heading, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current heading to the value provided. 

# Gyro Set Heading

Sets the Gyro Sensor's current heading to the specified heading. 

```cpp
Gyro.setHeading(heading, degrees);
```

## How To Use

`Gyro.setHeading` can be used to set the gyro's position to a heading in the range of **0** to **359.99**. 

This command is typically used to reset the orientation of the gyro when the heading is set to a value of 0.

`Gyro.setHeading` can accept decimals or integer inputs.

## Example

The below snippet sets the Gyro Sensor's current heading to 0 degrees.

```cpp
Gyro.setHeading(0, degrees);
```

<advanced>
</advanced>