category: sensing  
signature: ROTATION.position(degrees)  
device_class: rotation  
description: Reports a V5 Rotation Sensor's current position  

# Pyörimisasento

Antaa V5 Rotation Sensorin tämän hetkisen asennon.

```cpp
Rotation.position(units)
```

## Miten käytetään

`Rotation.position()` hyväksyy sekä **degrees** (asteita) että **turns** (kierroksia) ja anta sekä negatiivisia että positiivisia desimaali arvoja.

```cpp
Brain.Screen.print("%.2f", Rotation.position(degrees));
```

```cpp
Brain.Screen.print("%.2f", Rotation.position(turns));
```

<advanced>
</advanced>

