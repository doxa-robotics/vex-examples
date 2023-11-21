category: sensing  
signature: color.hue()  
device-class: colorsensor
description: Reports the hue of the color detected by a VEX IQ Color Sensor  

# Color Hue

Reports the hue of the color detected by a VEX IQ Color Sensor.

```python
color.hue()
```

## How To Use

`Color Hue` reports a range of values from **0 to 360** degrees, which represents the position of the color on the color wheel.

## Example

The example prints the hue of the color detected by the Color Sensor.

```python
brain.screen.print("Hue:", color.hue())
```

<advanced>
</advanced>