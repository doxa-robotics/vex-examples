category: sensing  
signature: OPTICAL.setLightPower(100, percent);  
device_class: optical  
description: Sets the intensity of a V5 Optical Sensor's LED  

# Optical aseta valon teho

Asettaa V5 Optical Sensorin LED valon tehon.

```cpp
Optical.setLightPower(power, percent);
```

## Miten käytetään

`Optical.setLightPower()`komennon avulla voi asettaa V5 Optical Sensor Led valon tehon.

Komento sallii arvot **0 - 100**  ensimmäisesä parametrissa.

Toinen parametri on yksikkö **percent** (%).

Mitä korkeampi arvo sitä kirkkaampi on LED valo ja päinvastoin himmeempi.

```cpp
Optical.setLightPower(100, percent);
Optical.setLight(ledState::on);
```

<advanced>
</advanced>







