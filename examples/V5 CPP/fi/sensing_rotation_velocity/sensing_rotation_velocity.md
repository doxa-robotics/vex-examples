category: sensing  
signature: ROTATION.velocity(rpm)  
device_class: rotation  
description: Reports the current velocity of a V5 Rotation Sensor  

# Rotation Nopeus

Antaa V5 Rotation Sensorin mittaaman nopeuden.

```cpp
Rotation.velocity(units)
```

## Miten käytetään

`Rotation.velocity()` hyväksyy sekä **rpm** (kierrosta minuutisa)  ja **dps** (asteita sekunnissa) ja antaa desimaaliarvona nopeuden.

```cpp
Brain.Screen.print("%.2f", Rotation.velocity(rpm));
```

```cpp
Brain.Screen.print("%.2f", Rotation.velocity(dps));
```

<advanced>
</advanced>



