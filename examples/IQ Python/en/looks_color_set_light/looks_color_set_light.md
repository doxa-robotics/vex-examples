category: looks  
signature: color.set_light(BRIGHTNESS, PERCENT)  
device_class: colorsensor  
description: Sets the brightness of the VEX IQ Color Sensor's light  

# Set Color Sensor Light

Sets the brightness of the VEX IQ Color Sensor's light. 

```python
color.set_light(BRIGHTNESS, PERCENT)
```

## How To Use

The Color Sensor has a light source that can be adjusted to help detect the color of an object or a surface.

`Set Color Sensor Light` accepts a range of **0 to 100** for the `BRIGHTNESS` parameter.

The higher the value is set, the brighter the Color Sensor's light source will shine.

## Example

The example below will set the brightness of the Color Sensor to 75%.

```python
color.set_light(75, PERCENT)
```

<advanced>
</advanced>
