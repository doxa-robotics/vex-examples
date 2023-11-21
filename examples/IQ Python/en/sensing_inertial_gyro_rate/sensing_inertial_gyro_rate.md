category: sensing  
signature: inertial.gyro_rate(AXIS, VelocityUnits.DPS)  
device_class: inertial  
description: Gets the rate of rotation for the specified axis (x, y, or z) on a VEX IQ (2nd generation) Brain's Inertial Sensor  

# Inertial Gyro Rate

Gets the rate of rotation for the specified axis (x, y, or z) on a VEX IQ (2nd generation) Brain's Inertial Sensor.

```python
brain_inertial.gyro_rate(AXIS, VelocityUnits.DPS)
```

## How To Use

Replace the **AXIS** parameter with one of the following options to get the gyro rate along an axis on the Inertial Sensor:

* **AxisType.XAXIS**: reports rotation when the Inertial Sensor rotates in the X-Axis (based on the orientation of the sensor)
* **AxisType.YAXIS**: reports rotation when the Inertial Sensor rotates in the Y-Axis (based on the orientation of the sensor)
* **AxisType.ZAXIS**: reports rotations when the Inertial Sensor rotates in the Z-Axis (based on the orientation of the sensor)

`Inertial Gyro Rate` is used to return a range from **-1000.0 to 1000.0** in dps (degrees per second). 

<advanced>
</advanced>
