category: sensing  
signature: inertial.orientation(OrientationType.ROLL , DEGREES)
description:  Gets an orientation angle of the inertial sensor. Reports the unit value specified by the parameter of the inertial sensor.

# Inertial Orientation

Gets an orientation angle of the inertial sensor. Reports the unit value specified by the parameter of the inertial sensor.

```don
inertial.orientation(OrientationType.ROLL, DEGREES)
```

## How To Use
The orientation reported is determined by the selected axis (x, y, or z).

* The X-axis represents pitch, which reports a value between -90 to +90 degrees.
* The Y-axis represents roll, which reports a value between -180 to +180 degrees)
* The Z-axis represents yaw, which reports a value between -180 to +180 degrees)

<advanced>
</advanced>
