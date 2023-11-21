category: sensing  
signature: gps.set_origin(0, 0, MM)  
description: Sets an origin point on a robot at which GPS Sensor positional data should be based upon.  

# GPS Set Origin

Sets an origin point on a robot at which GPS Sensor positional data should be based upon.

```python
gps.set_origin(X, Y, UNITS)
```

## How To Use

The `GPS.set_origin()` command can be used to allow GPS positional data to correspond to another point of a robot rather than the location of a GPS Sensor.

It is commonly used when a GPS Sensor is not located on the reference point of a robot (i.e. the point about which a robot rotates). This way, when the origin is set to the reference point, reported positional data would not change when a robot is rotating in-place.

The `X` parameter takes the X axis (i.e. the axis running through the sides of a GPS Sensor) while the `Y` parameter takes the Y axis offset distance to a reference point.

Either **MM** or **INCHES** are accepted for the `UNITS` parameter, depending on whether the x and y offset values are being passed as millimeters or inches, respectively.

## Example

```python
# Assuming a GPS Sensor is mounted 25mm forward from the reference point on a robot,
# we can set the origin on the GPS Sensor to have a Y offset of 25

gps.set_origin(0, 25, MM)
```

<advanced>
</advanced>
