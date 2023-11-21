category: sensing  
signature: OPTICAL.brightness()  
device_class: optical  
description: Reports the amount of light detected by an IQ Optical Sensor  

# Optical Brightness

Reports the amount of light detected by an IQ Optical Sensor.

```cpp
Optical.brightness()
```

## How To Use

`Optical.brightness()` reports a range of values from **0% to 100%**.

A large amount of light detected will report a high brightness value.

A small amount of light detected will report a low brightness value.

```cpp
Brain.Screen.print("%.2f", Optical.brightness());
```

<advanced>
</advanced>






