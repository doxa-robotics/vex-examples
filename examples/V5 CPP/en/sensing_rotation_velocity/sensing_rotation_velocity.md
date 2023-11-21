category: sensing  
signature: ROTATION.velocity(rpm)  
device_class: rotation  
description: Reports the current velocity of a V5 Rotation Sensor  

# Rotation Velocity

Reports the current velocity of a V5 Rotation Sensor.

```cpp
Rotation.velocity(units)
```

## How To Use

`Rotation.velocity()` accepts **rpm** or **dps** as units and reports decimal values.

```cpp
Brain.Screen.print("%.2f", Rotation.velocity(rpm));
```

```cpp
Brain.Screen.print("%.2f", Rotation.velocity(dps));
```

<advanced>
</advanced>



