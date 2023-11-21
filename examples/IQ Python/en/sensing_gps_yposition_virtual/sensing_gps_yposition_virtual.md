category: sensing  
signature: gps.y_position(MM)  
description: Reports the Y positional offset of a GPS Sensor or defined origin point from the center of a field.  

# GPS Y Position

Reports the Y positional offset of a GPS Sensor or defined origin point from the center of a field.

```python
gps.y_position(UNITS)
```

## How To Use

The `gps.y_position()` command reports the current Y positional offset of the V5 robot's turning reference (midpoint between the two front wheels) relative to the center of a field.

Values can be reported in mm or inches, depending on whether **MM** or **INCHES** is passed in the `UNITS` parameter.

## Example

```python
# Print the current Y position
brain.screen.print("GPS Y Position (MM): ", gps.y_position(MM))
```

<advanced>
</advanced>
