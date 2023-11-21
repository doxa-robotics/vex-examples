category: sensing  
signature: DISTANCE.isObjectDetected()  
device_class: distance  
description: Reports if an IQ Distance Sensor detects an object or surface in its range  

# Distance Object Detected

Reports if an IQ Distance Sensor detects an object or surface in its range.

```cpp
Distance.isObjectDetected()
```

## How To Use

`Distance.isObjectDetected()` returns **true** if an object or surface is detected in its range, and **false** if not.

The snippet below will print **TRUE** or **FALSE** depending on whether an object or surface is detected.

```cpp
Brain.Screen.print("%s", Distance.isObjectDetected() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>




