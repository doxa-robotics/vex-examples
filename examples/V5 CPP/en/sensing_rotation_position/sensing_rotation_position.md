category: sensing  
signature: ROTATION.position(degrees)  
device_class: rotation  
description: Reports a V5 Rotation Sensor's current position  

# Rotation Position

Reports a V5 Rotation Sensor's current position.

```cpp
Rotation.position(units)
```

## How To Use

`Rotation.position()` can accept **degrees** or **turns** as units and reports positive and negative decimal values.

```cpp
Brain.Screen.print("%.2f", Rotation.position(degrees));
```

```cpp
Brain.Screen.print("%.2f", Rotation.position(turns));
```

<advanced>
</advanced>

