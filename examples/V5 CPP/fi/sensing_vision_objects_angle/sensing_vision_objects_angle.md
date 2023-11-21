category: sensing  
signature: VISION.objects[0].angle  
device_class: vision  
description: Reports angle of a detected object from the Vision Sensor. 

# Kohteen kulma

Raportoi Vision -kameran havaitseman kohteen muodostaman kulman.
```cpp
Vision.objects[index].angle
```
## Miten käytetään

Tee järjestyksessä seuraavat toimenpideaskeleet, kun käytät `Vision.objects[index]` komentoa:

1. Määrittele Vision -kamerasi Laitteet - ja Kameran määritysikkunassa.
2. Käytä `Vision.takeSnapshot()` ottamaan kuvan ja etsimään siitä nimettyä merkkiä/värikoodia.
3. Käytä `Vision.objects[index].exists` tarkistamaan että halutun kohteen merkki/värikoodi löytyy kuvassa. 

Kun kohde löytyy, niin voit käyttää muita Vision -komentoja selvittämään tarkempia tietoja kohteeta. 

* Käytä **index** muuttujaa kiinnittämään kohde, josta haluat tarkempaa tietoa. Suurinesinekohde on aina edessä, jolloin se on  `Vision.objects[0]`.
* Käytä `Vision.objectCount` määrittämään motako samanlaista kohdetta löytyy halutulla merkillä/värikoodilla.
* Sitten voit käyttää muita ominaisuuksia: `angle`, `centerX`, `centerY`, `height`, `width` ja `exists`
## How To Use


---

`Vision.objects[index].angle` raportoi esineen kamerakulman arvolla **0 - 180 degrees**.

```cpp
Brain.screen.print(MyVision.objects[0].angle);
```

<advanced>
</advanced>