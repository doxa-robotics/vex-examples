category: sensing  
signature: GPS.setOrigin(0, 0, mm);  
device_class: gps  
description: Sets an origin point on a robot at which GPS Sensor positional data should be based upon.  

# GPS Set Origin

Sets an origin point on a robot at which GPS Sensor positional data should be based upon.

```cpp
GPS.setOrigin(x, y, units);
```

## How To Use

The `GPS.setOrigin()` command can be used to allow GPS positional data to correspond to another point of a robot rather than the location of a GPS Sensor.

It is commonly used when a GPS Sensor is not located on the reference point of a robot (i.e. the point about which a robot rotates). This way, when the origin is set to the reference point, reported positional data would not change when a robot is rotating in-place.

The `x` parameter takes the X axis (i.e. the axis running through the sides of a GPS Sensor) while the `y` parameter takes the Y axis offset distance to a reference point.

Either **mm** or **inches** are accepted for the `units` parameter, depending on whether the `x` and `y` offset values are being passed as millimeters or inches, respectively.

```cpp
// Assuming a GPS Sensor is mounted 25mm forward from the reference point of a robot,
// we can set the origin on the GPS Sensor to have a Y offset of 25
GPS.setOrigin(0, 25, mm);
```

<advanced>
</advanced>