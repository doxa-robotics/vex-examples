category: sensing  
signature: GPS.xPosition(mm)  
device_class: gps  
description: Reports the X positional offset of a GPS Sensor or defined origin point from the center of a field.  

# GPS X Position

Reports the X positional offset of a GPS Sensor or defined origin point from the center of a field.

```cpp
GPS.xPosition(units)
```

## How To Use

The `GPS.xPosition()` command reports the current X positional offset of a GPS Sensor or defined origin point relative to the center of a field.

If a `GPS.setOrigin()` command is used to set an origin point to a different part of a robot, the reported value will be the positional offset of the defined origin point from the center of a field.

Alternatively, the origin point can also be set in the GPS Sensor's configuration. This can be done by measuring the X and Y distances from the intended origin point to the GPS Sensor and filling in the X and Y offset settings, respectively.

Values can be reported in mm or inches as a *double*, depending on whether **mm** or **inches** is passed in the `units` parameter.

```cpp
Brain.Screen.print("GPS X Position (mm): %f", GPS.xPosition(mm));
```

<advanced>
</advanced>