category: sensing  
signature: Distance.distance(units)  
device-class: sonar
description: Reports the distance of the nearest object from the VEX IQ Distance Sensor.

# Etäisyysanturi etäisyys esineestä

Raportoi lähimmän esineen ja etäisyysanturin välisen välimatkan.

```cpp
Distance.distance(units)
```

## Miten käytetään

`Distance.distance` raportoi välimatkat väliltä **24mm - 1000mm** tai **1 tuumaa - 40 tuumaa**.

Ensimmäinen osa komentoa on nimetty etäisyysanturi.

```cpp
Distance6.distance(mm)
Distance8.distance(inches)
```

Valitse yksikkö, jolla välimatka `Distance.distance` mitataan:  **tuuma** tai **mm**. 

```cpp
Distance6.distance(mm)
Distance8.distance(inches)
```

<advanced>
</advanced>