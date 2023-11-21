category: sensing  
signature: INERTIAL.acceleration(xaxis);  
device_class: inertial  
description: Reports the acceleration value from one of the axes (x, y, or z) on the Inertial Sensor.  

# Inertial kiihtyvyys

Antaa Inertial Sensorin mittaaman kiihtyvyyden yhdellä akselilla (x, y, tai z) on the Inertial Sensor.  

* **X-akseli** -suuntaan Inertial Sensori mittaa kiihtyvyyttä , kun robotti liikkuu akselilla **eteen - taakse**
* **Y-akseli** -suuntaan Inertial Sensori mittaa kiihtyvyyttä , kun robotti liikkuu akselilla **sivulta sivulle**
* **Z-akseli** -suuntaan Inertial Sensori mittaa kiihtyvyyttä , kun robotti liikkuu akselilla **ylös-alas**

```cpp
Inertial.acceleration(axis)
```

## Miten käytetään

Komentoa voidaan käyttää toisten komentojen sisällä kuten tulsota-komennossa tai ohjauslauseissa osana ehtolausetta ja älä käytä puolipistettä.

`Inertial.acceleration()` antaa arvot desimaalilukuna (muotoa *double*) välillä **-4.0 - 4.0 Gs**.

```cpp
Brain.Screen.print("%f", Inertial1.acceleration(xaxis));
Brain.Screen.print("%f", Inertial1.acceleration(yaxis));
Brain.Screen.print("%f", Inertial1.acceleration(zaxis));
```
<advanced>
</advanced>
