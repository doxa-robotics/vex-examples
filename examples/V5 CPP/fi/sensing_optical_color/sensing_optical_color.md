category: sensing  
signature: OPTICAL.color()  
device_class: optical  
description:  Returns the color detected by a V5 Optical Sensor  

# Optical väri

Palauttaa värin nimen, jonka V5 Optical Sensori tunnistaa.

```cpp
Optical.color()
```

## Miten käytetään

`Optical.color()` palauttaa lähimmän värin, jonka se tunnistaa esineestä.

Seuraavia värejä voi käytttää vertailuun, mitä V5 Optical Sensori havaitsee:

* black (musta)
* white (valkoinen)
* red (punainen)
* green (vihreä)
* blue (sininen)
* yellow (keltainen)
* orange (oranssi)
* purple (purppuran punainen)
* cyan (syaani vaalen sininen)

```cpp
if (Optical.color() == red) {
  Brain.Screen.print("Red object detected!");
}
```

<advanced>
</advanced>







