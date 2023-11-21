category: sensing  
signature: potentiometer.angle(UNITS)
description: Returns the angular position of the Potentiometer.

# Potentiometer Angle

Returns the angular position of the Potentiometer.

```don
potentiometer.angle(UNITS)
```

## How To Use

`potentiometer.angle` returns a decimal value to report the angular position of the Potentiometer.

The `UNITS` parameter accepts either **DEGREES** or **PERCENT** as an argument.

If the provided `UNITS` is in **DEGREES**, the range of returned values will be from **0.0 to 250.0 degrees** for a V5 Potentiometer, and from **0.0 to 330.0** degrees for a V5 Potentiometer V2.

Alternatively, the returned values will range from **0 to 100%** if the provided `UNITS` is in **PERCENT**.

<advanced>
</advanced>
