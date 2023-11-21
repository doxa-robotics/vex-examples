category: sensing  
signature: GYRO.rotation(degrees)  
device_class: gyro  
description: Reports the 3-Wire Gyro Sensor's current angle of rotation in degrees.

# Gyro kääntymiskulma

Antaa 3-lanka Gyro Sensorin antaman kääntymiskulman asteina.

```cpp
Gyro.rotation(degrees)
```

## Miten käytetään

`Gyro.rotation(degrees)` antaa positiivisen **positive** arvon kun gyro kääntyy myötäpäivään.

`Gyro.rotation(degrees)` antaa nagatiivisen **negative** arvon kun gyro kääntyy vastapäivään.

```cpp
waitUntil(Gyro.rotation(degrees) > 180);
```
<advanced>
</advanced>
