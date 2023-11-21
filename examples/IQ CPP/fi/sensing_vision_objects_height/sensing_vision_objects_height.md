category: sensing  
signature: VISION.objects[0].height;  
device_class: vision  
description: Reports the height of a detected object from the Vision Sensor.

# Kohde korkeus

Aataa Vision -kameran havaitun kohteen korkeuden.

```cpp
Vision.objects[index].height
```

## Miten käytetään

Tee järjestyksessä seuraavat toimenpideaskeleet, kun käytät `Vision.objects[index]` komentoa:

1. Määrittele Vision -kamerasi Laitteet - ja Kameran määritysikkunassa.
2. Käytä `Vision.takeSnapshot()` ottamaan kuvan ja etsimään siitä nimettyä merkkiä/värikoodia.
3. Käytä `Vision.objects[index].exists` tarkistamaan että halutun kohteen merkki/värikoodi löytyy kuvassa. 

Kun kohde öytyy, niin voit käyttää muita Vision -komentoja selvittämään tarkempia tietoja kohteeta. 

* Käytä **indeksi** muuttujaa kiinnittämään kohde, josta haluat tarkempaa tietoa. Suurinesinekohde on aina edessä, jolloin se on  `Vision.objects[0]`.
* Käytä `Vision.objectCount` määrittämään motako samanlaista kohdetta löytyy halutulla merkillä/värikoodilla.
* Sitten voit käyttää muita ominaisuuksia: `kulma`, `keskipisteX`, `keskipisteY`, `korkeus`, `leveys` ja `on olemassa`.

---

`Vision.objects[index].height` antaa kohteen korkeuden pikseleinä arvovälillä **2 - 212 px**.

```cpp
Brain.Screen.print(MyVision.objects[3].height);
```

<advanced>
</advanced>