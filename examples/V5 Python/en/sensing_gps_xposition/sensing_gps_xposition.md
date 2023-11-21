category: sensing  
signature: gps.x_position(MM)  
description: Reports the X positional offset of a GPS Sensor or defined origin point from the center of a field.  

# GPS X Position

Reports the X positional offset of a GPS Sensor or defined origin point from the center of a field.

```python
gps.x_position(UNITS)
```

## How To Use

The `gps.x_position()` command reports the current X positional offset of a GPS Sensor or defined origin point relative to the center of a field.

If a `gps.set_origin()` command is used to set an origin point to a different part of a robot, the reported value will be the positional offset of the defined origin point from the center of a field.

Alternatively, the origin point can also be set in the GPS Sensor's configuration. This can be done by measuring the X and Y distances from the intended origin point to the GPS Sensor and filling in the X and Y offset settings, respectively.

Values can be reported in mm or inches, depending on whether **MM** or **INCHES** is passed in the `UNITS` parameter.

## Example

```python
# Print the current X position of a GPS Sensor
brain.screen.print("GPS X Position (MM): ", gps.x_position(MM))
```

<advanced>
</advanced>
