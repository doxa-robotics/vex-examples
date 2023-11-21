category: sensing  
signature: OPTICAL.hue()  
device_class: optical  
description: Reports the hue of the object detected by an IQ Optical Sensor  

# Optical Hue

Reports the hue of the object detected by an IQ Optical Sensor.

```cpp
Optical.hue()
```

## How To Use

`Optical.hue()` reports a range of values from **0 to 359**, which represents the location of the detected color on a color wheel.

```cpp
Brain.Screen.print("%.2f", Optical.hue());
```

<advanced>
</advanced>







