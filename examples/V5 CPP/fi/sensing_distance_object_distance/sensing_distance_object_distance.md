category: sensing  
signature: DISTANCE.objectDistance(inches)  
device_class: distance  
description: Reports the distance of the nearest object or surface from a V5 Distance Sensor  

# Distance Object Distance

Reports the distance of the nearest object or surface from a V5 Distance Sensor.

```cpp
Distance.objectDistance(units)
```

## How To Use

`Distance.objectDistance()` accepts **mm** or **inches** as units and reports a range from **20 mm to 2000 mm** (~0.8 inches to 79.0 inches ) as a decimal value.

```cpp
Brain.Screen.print("%.2f", Distance.objectDistance(inches));
```

```cpp
Brain.Screen.print("%.2f", Distance.objectDistance(mm));
```
<advanced>
</advanced>





