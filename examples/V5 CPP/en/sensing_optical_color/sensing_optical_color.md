category: sensing  
signature: OPTICAL.color()  
device_class: optical  
description:  Returns the color detected by a V5 Optical Sensor  

# Optical Color

Returns the color detected by a V5 Optical Sensor.

```cpp
Optical.color()
```

## How To Use

`Optical.color()` returns the closest color match base on the hue of a detected object.

The following colors can be used as a comparison to the color detected by a V5 Optical Sensor:
* black
* white
* red
* green
* blue
* yellow
* orange
* purple
* cyan

```cpp
if (Optical.color() == red) {
  Brain.Screen.print("Red object detected!");
}
```

<advanced>
</advanced>







