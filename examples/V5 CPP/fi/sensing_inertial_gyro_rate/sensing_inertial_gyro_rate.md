category: sensing  
signature: INERTIAL.gyroRate(xaxis, dps)  
device_class: inertial  
description: Gets the rate of rotation for the specified axis (x, y, or z) on the Inertial Sensor  

# Inertial Gyro nopeusarvo

Antaa Inertial Sensorin mittaaman käännöksen nopeusarvon akselilla (x, y, or z).

* **X-akseli** suunnassa nopeusarvon, kun Inertial Sensori kääntyy X-Akselilla (riippuen sensorin suunnasta)
* **Y-akseli** suunnassa nopeusarvon, kun Inertial Sensori kääntyy Y-Akselilla (riippuen sensorin suunnasta)
* **Z-akseli** suunnassa nopeusarvon, kun Inertial Sensori kääntyy Z-Akselilla (riippuen sensorin suunnasta)

```cpp
Inertial.gyroRate(axis, dps)
```

## Miten käytetään

Komentoa voi käyttää muiden komentojen sisällä mm tulosta-komennossa taitoistorakenteiden ehtolauseissa ja älä käytä puolipistettä.

`Inertial.gyroRate()` antaa arvot välillä **-1000.0 - 1000.0** dps (astetta sekunnissa). 

```cpp
Brain.Screen.print("%f", Inertial.gyroRate(xaxis, dps));
Brain.Screen.print("%f", Inertial.gyroRate(yaxis, dps));
Brain.Screen.print("%f", Inertial.gyroRate(zaxis, dps));
```

<advanced>
</advanced>
