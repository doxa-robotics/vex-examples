category: looks  
signature: Color.setLight(50, percent);  
device_class: Color Sensor  
description: Sets the brightness of the VEX IQ Color Sensor's light.  

# Set Color Sensor Light

Sets the brightness of the VEX IQ Color Sensor's light. 

```cpp
Color.setLight(brightness, percent);
```

## How To Use

The Color Sensor has a light source that can be adjusted to help detect the color of an object or a surface.

`Color.setLight` accepts a range of **0 to 100** for the `brightness` parameter.

The higher the value is set, the brighter the Color Sensor's light source will shine.

## Example

The example below will set the brightness of the Color Sensor to 75%.

```cpp
Color.setLight(75, percent);
```

<advanced>
</advanced>
