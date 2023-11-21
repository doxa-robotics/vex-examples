category: sensing  
signature: inertial.set_heading(HEADING, DEGREES)  
device_class: inertial  
description: Sets a VEX IQ (2nd generation) Brain's Inertial Sensor's current heading position to a specified heading  

# Inertial Set Heading

Sets a VEX IQ (2nd generation) Brain's Inertial Sensor's current heading position to a specified heading.

```python
brain_inertial.set_heading(HEADING, DEGREES)
```

## How To Use

`Inertial Set Heading` can be used to set the IQ (2nd generation) Brain's Inertial Sensor's position to any clockwise-positive heading. This command is typically used to reset the orientation of the IQ (2nd generation) Brain Inertial Sensor when the heading is set to a value of 0.

`Inertial Set Heading` accepts a range of **0.0 to 359.99** for the **HEADING** parameter.

<advanced>
</advanced>
