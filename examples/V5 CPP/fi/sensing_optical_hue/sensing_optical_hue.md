category: sensing  
signature: OPTICAL.hue()  
device_class: optical  
description: Reports the hue of the object detected by a V5 Optical Sensor  

# Optical Värisävu

Antaa esineen värisävyn, jonka V5 Optical Sensori tunnistaa.

```cpp
Optical.hue()
```

## Miten käytetään

`Optical.hue()` antaa värisävyn arvon välillä **0 to 359** ja vastaavan värin voi tarksitaa Vex värispektrikuvasta.

```cpp
Brain.Screen.print("%.2f", Optical.hue());
```

<advanced>
</advanced>







