category: sensing  
signature: gyro.set_rotation(ROTATION, DEGREES)  
device_class: gyro  
description: Sets a VEX IQ Gyro Sensor's current angle of rotation to the specified rotation  

# Gyro Set Rotation

Sets a VEX IQ Gyro Sensor's current angle of rotation to the specified rotation. 

```python
gyro.set_rotation(ROTATION, DEGREES)
```

## How To Use

The `Gyro Set Rotation` command can be used to set a Gyro Sensor's angle of rotation to any given positive (counter-clockwise increasing) or negative (clockwise decreasing) value.

`Gyro Set Rotation` accepts a range of any positive or negative decimal or integer as the specified **ROTATION**.

## Example

The example below sets the rotation of the Gyro Sensor to -45 degrees.

```python
gyro.set_rotation(-45, DEGREES)
```

<advanced>
</advanced>