category: sensing  
signature: DISTANCE.objectVelocity()  
device_class: distance  
description: Reports the velocity of a detected object in m/s  

# Kohteen nopeus

Antaa havaitun kohteen nopeuden yksikössä m/s.

```cpp
Distance.objectVelocity()
```

## Miten käytetään

`Distance.objectVelocity()` antaa tänhetkisen kohteen nopeuden yksikössä m/s (metriä sekunnissa).


```cpp
Brain.Screen.print("%.2f", Distance.objectVelocity());
```

<advanced>
</advanced>






