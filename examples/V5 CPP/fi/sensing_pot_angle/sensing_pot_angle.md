category: sensing  
signature: POTENTIOMETER.angle(units)  
device_class: pot  
description: Returns the angular position of the Potentiometer.

# Potentiometrin kulma

Palauttaa Potentiometertrin mittaaman kulman.

```cpp
Potentiometer.angle(units)
```

## Miten käytetään

`Potentiometer.angle()` antaa desimaaliarvon (muotoa *double*) Potentiometrin asentokulmalle.

Komentoa voi käyttää arvona muissa komennoissa (kuten tulosta komennossa) tao ohjauslausekkeiden ehdoissa.

Aseta **degrees** (astetta) yksiköksi `units` parametriin ja arvot saa volla välillä **0.0 - 250.0 astetta**.

Jos yksikkö on **percent** (%), arvot ovat välillä **0 - 100%**.

```cpp
Brain.Screen.print("%f", PotentiometerA.angle(degrees));
```

<advanced>
</advanced>