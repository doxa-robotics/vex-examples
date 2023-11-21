category: sensing  
signature: OPTICAL.setLight(ledState::on);  
device_class: optical  
description: Sets the state of the V5 Optical Sensor's LED    

# Optical aseta valo päälle

Asetaa V5 Optical Sensorin LED valon päälle.

```cpp
Optical.setLight(ledState);
```

## Miten käytetään

`Optical.setLight()`komentoa käytetään laittaan V5 Optical Sensor LED valo päälle.

Komento hyväksyy vaihtoehdot **ledState::on** (päällä) tai **ledState::off** (pois päältä) parametrissa.

**ledState::on** laittaa LED valon päälle.

**ledState::off** ottaa  LED valon pois.

```cpp
Optical.setLight(ledState::on);
wait(2, seconds);
Optical.setLight(ledState::off);
```

<advanced>
</advanced>







