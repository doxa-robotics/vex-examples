category: sensing  
signature: gyro.set_heading(0, DEGREES)
description: Sets the Gyroscopic (Gyro) sensor's current heading position to a set value.

# Set Gyro Heading

Sets the Gyroscopic (Gyro) Sensor's current heading position to a set value.
 
```don
gyro.set_heading(HEADING, DEGREES)
```

## How To Use

The set gyro heading command can be used to set the Gyro's position to any clockwise heading.

This command is typically used reset the heading orientation of the Gyro sensor when value is set to 0.

The `HEADING` parameter accepts a range of 0.0 to 359.99 degrees.

The set heading command can accept decimals, integers, or numeric values.

<advanced>
</advanced>
