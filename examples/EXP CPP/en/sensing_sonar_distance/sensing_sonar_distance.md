category: sensing  
signature: RANGEFINDER.distance(mm)  
device_class: sonar  
description: Reports the distance of the nearest object from the Ultrasonic Range Finder sensor.

# RangeFinder Distance

Reports the distance of the nearest object from the Ultrasonic Range Finder sensor.

```cpp
RangeFinder.distance(units)
```

## How To Use

`RangeFinder.distance()` reports a range from **30mm to 3000mm** if the unit specified is `mm`, or **2 inches to 115 inches** if the unit specified is `inches`.

```cpp
if (RangeFinderC.distance(mm) < 400.0){
    Drivetrain.stop();
}
```
<advanced>
</advanced>