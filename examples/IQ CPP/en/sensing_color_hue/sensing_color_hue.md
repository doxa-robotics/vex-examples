category: sensing  
signature: Color.hue()  
device-class: colorsensor
description: Reports the hue of the color detected by the VEX IQ Color Sensor.

# Color Hue

Reports the hue of the color detected by the VEX IQ Color Sensor.

```cpp
Color.hue()
```

## How To Use

`Color.hue` reports a range of values from **0** to **360** degrees, which represents the position of the color on the color wheel.

## Example

The example prints the hue of the color detected by the Color Sensor.

```cpp
Brain.Screen.print("Hue: %.0f", Color.hue());
```

<advanced>
</advanced>