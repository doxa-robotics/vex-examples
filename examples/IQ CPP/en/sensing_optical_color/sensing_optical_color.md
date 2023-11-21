category: sensing  
signature: OPTICAL.color()  
device_class: optical  
description:  Returns the color detected by an IQ Optical Sensor  

# Optical Color

Returns the color detected by an IQ Optical Sensor.

```cpp
// IQ (1st generation)
Optical.colorname()

// IQ (2nd generation)
Optical.color()
```

## How To Use

The `Optical Color` command returns the closest color match base on the hue of a detected object.

The following colors can be used as a comparison to the color detected by an IQ Optical Sensor:
- red
- green
- blue
- yellow
- orange
- purple
- cyan

### IQ (1st generation) Brain

```cpp
if (Optical.colorname() == red) {
  Brain.Screen.print("Red object detected!");
}
```

### IQ (2nd generation) Brain

```cpp
if (Optical.color() == red) {
  Brain.Screen.print("Red object detected!");
}
```

<advanced>
</advanced>







