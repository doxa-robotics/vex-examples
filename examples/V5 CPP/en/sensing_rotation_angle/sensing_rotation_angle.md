category: sensing  
signature: ROTATION.angle()  
device_class: rotation  
description: Reports a V5 Rotation Sensor's current angle of rotation in degrees  

# Rotation Angle

Reports a V5 Rotation Sensor's current angle of rotation in degrees.

```cpp
Rotation.angle()
```

## How To Use

The `Rotation.angle()` command reports values in the range of **0.00** to **359.99**.


```cpp
Brain.Screen.print("%.2f", Rotation.angle());
```

<advanced>
</advanced>
