category: sensing  
signature: INERTIAL.acceleration(xaxis);  
device_class: inertial  
description: Reports the acceleration value from one of the axes (x, y, or z) on the Inertial Sensor.  

# Inertial Acceleration

Reports the acceleration value from one of the axes (x, y, or z) on the Inertial Sensor.  

* The **X-axis** reports acceleration when the Inertial Sensor moves **forward to backward**
* The **Y-axis** reports acceleration when the Inertial Sensor moves **side to side**
* The **Z-axis** reports acceleration when the Inertial Sensor moves **up to down**

```cpp
Inertial.acceleration(axis)
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Inertial.acceleration()` returns a decimal value (as a *double*) that ranges from **-4.0 to 4.0 Gs**.

```cpp
Brain.Screen.print("%f", Inertial1.acceleration(xaxis));
Brain.Screen.print("%f", Inertial1.acceleration(yaxis));
Brain.Screen.print("%f", Inertial1.acceleration(zaxis));
```
<advanced>
</advanced>
