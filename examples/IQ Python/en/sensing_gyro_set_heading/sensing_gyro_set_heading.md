category: sensing  
signature: gyro.set_heading(HEADING, DEGREES)  
device_class: gyro  
description: Sets a VEX IQ Gyro Sensor's current heading to the specified heading  

# Gyro Set Heading

Sets a VEX IQ Gyro Sensor's current heading to the specified heading.

```python
gyro.set_heading(HEADING, DEGREES)
```

## How To Use

`Gyro Set Heading` can be used to set the gyro's position to a heading in the range of **0 to 359.99** degrees. 

This command is typically used to reset the orientation of the gyro when the heading is set to a value of 0.

`Gyro Set Heading` can accept decimal or integer inputs.

## Example

The below snippet sets the Gyro Sensor's current heading to 0 degrees.

```python
gyro.set_heading(0, DEGREES)
```

<advanced>
</advanced>