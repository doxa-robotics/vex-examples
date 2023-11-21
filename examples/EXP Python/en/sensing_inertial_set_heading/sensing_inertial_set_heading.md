category: sensing  
signature: inertial.set_heading(0, DEGREES)
description: Sets the Inertial sensor's current heading position to a set value.

# Set Inertial Heading

Sets the Inertial sensor's current heading position to a set value.

```don
inertial.set_heading(HEADING, DEGREES)
```

## How To Use

`inertial.set_heading` can be used to set the Inertial Sensor's position to any clockwise heading. This command is typically used to reset the orientation of the Inertial Sensor when the heading is set to a value of 0.

`inertial.set_heading` is typically used to reset the heading orientation of the Inertial sensor when a value is set to 0.

`inertial.set_heading` accepts a range of 0.0 to 359.99 degrees.

`inertial.set_heading` can accept decimals, integers, or numeric values.


<advanced>
</advanced>
