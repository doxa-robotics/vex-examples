category: sensing  
signature: VISION.objects[0].centerY  
device_class: vision  
description: Reports the Y coordinate of the center of a detected object from the Vision Sensor.

# Kohteen KeskipisteY

Antaaa y-akselilla Vision -kameran havaitseman kohteen keskipisteen.

```cpp
Vision.objects[index].centerY
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

`Vision.objects[index].centerY` raportoi Y -akselin kohteen keskipisteen arvolla **0 - 211 px**.

```cpp
Brain.Screen.print(MyVision.objects[2].centerY);
```

<advanced>
</advanced>