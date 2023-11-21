category: sensing  
signature: ROTATION.angle()  
device_class: rotation  
description: Reports a V5 Rotation Sensor's current angle of rotation in degrees  

# Rotation Angle

Antaa V5 Rotation Sensorin mittaaman pyörimiskulman asteina.

```cpp
Rotation.angle()
```

## Miten käytetään

`Rotation.angle()` antaa arvot välillä **0.00** - **359.99**.


```cpp
Brain.Screen.print("%.2f", Rotation.angle());
```

<advanced>
</advanced>
