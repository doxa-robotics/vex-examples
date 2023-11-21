category: sensing  
signature: inertial.gyro_rate(AxisType.XAXIS, VelocityUnits.DPS)
description:  Gets the rate of rotation from one of the axes (x, y, or z) on the Inertial Sensor.

# Inertial Gyro Rate

Gets the rate of rotation from one of the axes (x, y, or z) on the Inertial Sensor.

```don
inertial.gyro_rate(AxisType.XAXIS, VelocityUnits.DPS)
```

## How To Use

Gyro rate reports a range from **-1000.0 to 1000.0** in dps (degrees per second).

Choose which axis to use.

* The X-axis reports rate of rotation when the Inertial Sensor rotates in the X-Axis (based on the orientation of the sensor)
* The Y-axis reports rate of rotation when the Inertial Sensor rotates in the Y-Axis (based on the orientation of the sensor)
* The Z-axis reports rate of rotation when the Inertial Sensor rotates in the Z-Axis (based on the orientation of the sensor)


<advanced>
</advanced>
