category: sensing  
signature: Color.hue()  
device-class: colorsensor
description: Reports the hue of the color detected by the VEX IQ Color Sensor.

# Värisävy

Raportoi VEX IQ värisensorin havaitseman esineen värisävyn.

```cpp
Color.hue()
```

## Miten käytetään

`Color.hue` raportoi värisävyn arvon välillä **0** - **360** astetta VEX värispetrillä.

## Esimerkki

Esimerkissä Aivojen näytölle tulostetaan havaittu värisävyn numeroarvo.

```cpp
Brain.Screen.print("Hue: %.0f", Color.hue());
```

<advanced>
</advanced>