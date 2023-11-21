category: sensing  
signature: gps.gyro_rate(AxisType.XAXIS, VelocityUnits.DPS)  
description: Reports the rate of rotation from the specified axis on a GPS Sensor.  

# GPS Gyro Rate

Reports the rate of rotation from the specified axis on a GPS Sensor.

```python
gps.gyro_rate(AXIS, UNITS)
```

## How To Use

The `gps.gyro_rate()` command reports the rate of rotation on an axis with the range of values reported between **-1000** to **1000** if **VelocityUnits.DPS** is used as the `UNITS` parameter, or between **-167** to **167** if **VelocityUnits.RPM** is used.

The `AXIS` parameter accepts the following values for specifying which axis to get rate of rotation from:

* **AxisType.XAXIS**: reports the rate of rotation when a GPS Sensor rotates in the X-Axis (based on the orientation of the sensor)

* **AxisType.YAXIS**: reports the rate of rotation when a GPS Sensor rotates in the Y-Axis (based on the orientation of the sensor)

* **AxisType.ZAXIS**: reports the rate of rotation when a GPS Sensor rotates in the Z-Axis (based on the orientation of the sensor)

## Example

```python
# Print gyro rate values from all GPS Sensor axes in a loop
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("GPS Gyro Rate - X Axis: ", gps.gyro_rate(AxisType.XAXIS, VelocityUnits.DPS))
    brain.screen.next_row()
    brain.screen.print("GPS Gyro Rate - Y Axis: ", gps.gyro_rate(AxisType.YAXIS, VelocityUnits.DPS))
    brain.screen.next_row()
    brain.screen.print("GPS Gyro Rate - Z Axis: ", gps.gyro_rate(AxisType.ZAXIS, VelocityUnits.DPS))
    brain.screen.next_row()
    wait(0.1, SECONDS)
```

<advanced>
</advanced>
