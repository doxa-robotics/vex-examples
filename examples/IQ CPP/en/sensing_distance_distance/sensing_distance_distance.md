category: sensing  
signature: Distance.distance(units)  
device-class: sonar
description: Reports the distance of the nearest object from the VEX IQ Distance Sensor.

# Distance From

Reports the distance of the nearest object from the VEX IQ Distance Sensor.

```cpp
Distance.distance(units)
```

## How To Use

`Distance.distance` reports a range from **24mm to 1000mm** or **1 inch to 40 inches**.

The first part of the command is the device instance.

```cpp
Distance6.distance(mm)
Distance8.distance(inches)
```

Specify whether the value returned by `Distance.distance` is reported in **inches** or **mm** (millimeters). 

```cpp
Distance6.distance(mm)
Distance8.distance(inches)
```

<advanced>
</advanced>