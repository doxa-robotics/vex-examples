category: sensing  
signature: GPS.gyroRate(xaxis, dps)  
device_class: gps  
description: Reports the rate of rotation from the specified axis on a GPS Sensor.  

# GPS Gyro Rate

Reports the rate of rotation from the specified axis on a GPS Sensor.

```cpp
GPS.gyroRate(axis, units)
```

## How To Use

`GPS.gyroRate()` reports the rate of rotation on an axis as a *double*, with the range of values reported between **-1000** to **1000** if **dps** is used as the `units` parameter, or between **-167** to **167** if **rpm** is used.

The `axis` parameter accepts the following values for specifying which axis to get rate of rotation from:

* **xaxis**: reports the rate of rotation when a GPS Sensor rotates in the X-Axis (based on the orientation of the sensor)

* **yaxis**: reports the rate of rotation when a GPS Sensor rotates in the Y-Axis (based on the orientation of the sensor)

* **zaxis**: reports the rate of rotation when a GPS Sensor rotates in the Z-Axis (based on the orientation of the sensor)

## Example

```cpp
// Print all gyro rate values in a loop
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("GPS Gyro Rate - X Axis: %f", GPS.gyroRate(xaxis, dps));
  Brain.Screen.newLine();
  Brain.Screen.print("GPS Gyro Rate - Y Axis: %f", GPS.gyroRate(yaxis, dps));
  Brain.Screen.newLine();
  Brain.Screen.print("GPS Gyro Rate - Z Axis: %f", GPS.gyroRate(zaxis, dps));
  Brain.Screen.newLine();
  wait(0.1, seconds);
}
```

<advanced>
</advanced>