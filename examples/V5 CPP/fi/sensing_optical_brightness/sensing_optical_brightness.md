category: sensing  
signature: OPTICAL.brightness()  
device_class: optical  
description: Reports the amount of light detected by a V5 Optical Sensor  

# Optical.brightness()

Antaa V5 Optical Sensorin havaitseman valon määrän.

```cpp
Optical.brightness()
```

## Miten käytetään

`Optical.brightness()` anta arvot välillä **0% - 100%**.

Mitä enemmän valoa sensori näkee sitä korkeampi on arvo.

Huono valaistus aantaa matalan arvon.

```cpp
Brain.Screen.print("%.2f", Optical.brightness());
```

<advanced>
</advanced>






