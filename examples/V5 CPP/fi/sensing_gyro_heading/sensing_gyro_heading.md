category: sensing  
signature: GYRO.heading(degrees)  
device_class: gyro  
description: Reports the 3-Wire Gyro Sensor's current heading in degrees.

# Gyro Ajosuunta

Antaa 3-lanka Gyro Sensorin ajosuunnan tällä hetkellä asteina.

```cpp
Gyro.heading(degrees)
```

## Miten käytetään

`Gyro.heading(degrees)` komennossa arvot kasvavat myötäpäivään kääntyessä.

`Gyro.heading(degrees)` anta arvot välillä **0.00 - 359.99**.

```cpp
waitUntil(Gyro.heading(degrees) > 180);
```
<advanced>
</advanced>