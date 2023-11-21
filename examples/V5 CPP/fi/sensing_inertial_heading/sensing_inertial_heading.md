category: sensing  
signature: INERTIAL.heading(degrees)  
device_class: inertial  
description: Reports the V5 Inertial Sensor's current heading in degrees.

# Inertial ajosuunta

ANtaa V5 Inertial Sensorin mittaaman ajosuunnan asteina.

```cpp
Inertial.heading(degrees)
```

## Miten käytetään

Komentoa voi kättää muiden komentojen sisällä mm tulsota -komennossa tai toistorakenteiden ehtolauseissa ja älä käytä puolipistettä.

`Inertial.heading(degrees)` komennon arvo kasvaa kun ajosuuntaa kääntyy myötäpäivään.

`Inertial.heading(degrees)` antaa arvon väliltä **0.00 - 359.99 astetta**

```cpp
waitUntil(Inertial.heading(degrees) > 180);
```
<advanced>
</advanced>
