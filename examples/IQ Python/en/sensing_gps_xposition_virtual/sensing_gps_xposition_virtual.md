category: sensing  
signature: gps.x_position(MM)  
description: Reports the X positional offset of a GPS Sensor or defined origin point from the center of a field.  

# GPS X Position

Reports the X positional offset of a GPS Sensor or defined origin point from the center of a field.

```python
gps.x_position(UNITS)
```

## How To Use

The `gps.x_position()` command reports the current X positional offset of the V5 robot's turning reference (midpoint between the two front wheels) relative to the center of a field.

Values can be reported in mm or inches, depending on whether **MM** or **INCHES** is passed in the `UNITS` parameter.

## Example

```python
# Print the current X position
brain.screen.print("GPS X Position (MM): ", gps.x_position(MM))
```

<advanced>
</advanced>
