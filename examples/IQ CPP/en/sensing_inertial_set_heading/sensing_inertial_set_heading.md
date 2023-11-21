category: sensing  
signature: INERTIAL.setHeading(0, degrees);  
device_class: inertial  
description: Sets the IQ (2nd generation) Brain Inertial sensor's current heading position to a specified value.

# Inertial Set Heading

Sets the IQ (2nd generation) Brain Inertial sensor's current heading position to a specified value.

```cpp
BrainInertial.setHeading(0, degrees);
```

## How To Use

`BrainInertial.setHeading()` can be used to set the IQ (2nd generation) Brain Inertial sensor's position to any clockwise-positive heading. This command is typically used to reset the orientation of the IQ (2nd generation) Brain Inertial sensor when the heading is set to a value of 0.

`BrainInertial.setHeading()` accepts a range of **0.0 to 359.99** degrees.

`BrainInertial.setHeading()` can accept decimals, integers, or other commands that return a numeric value.

<advanced>
</advanced>
