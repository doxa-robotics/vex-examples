category: sensing  
signature: INERTIAL.gyroRate(xaxis, dps)  
device_class: inertial  
description: Gets the rate of rotation for the specified axis (x, y, or z) on the Inertial Sensor  

# Inertial Gyro Rate

Gets the rate of rotation for the specified axis (x, y, or z) on the Inertial Sensor.

* The **X-axis** reports rotation when the Inertial Sensor rotates in the X-Axis (based on the orientation of the sensor)
* The **Y-axis** reports rotation when the Inertial Sensor rotates in the Y-Axis (based on the orientation of the sensor)
* The **Z-axis** reports rotations when the Inertial Sensor rotates in the Z-Axis (based on the orientation of the sensor)

```cpp
Inertial.gyroRate(axis, dps)
```

## How To Use 

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon

`Inertial.gyroRate()` is used to return a range from **-1000.0 to 1000.0** in dps (degrees per second). 

```cpp
Brain.Screen.print("%f", Inertial.gyroRate(xaxis, dps));
Brain.Screen.print("%f", Inertial.gyroRate(yaxis, dps));
Brain.Screen.print("%f", Inertial.gyroRate(zaxis, dps));
```

<advanced>
</advanced>
