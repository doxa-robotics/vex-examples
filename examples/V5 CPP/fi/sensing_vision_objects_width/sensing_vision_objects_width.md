category: sensing  
signature: VISION.objects[0].width;  
device_class: vision  
description: Reports the width of a detected object from the Vision Sensor.

# Vision.objects[index].width

Raportoi Vision -kameran havaitseman kohteen leveyden

```cpp
Vision.objects[index].width
```


## Miten käytetään

Tee järjestyksessä seuraavat toimenpideaskeleet, kun käytät `Vision.objects[index]` komentoa:

1. Määrittele Vision -kamerasi Laitteet - ja Kameran määritysikkunassa.
2. Käytä `Vision.takeSnapshot()` ottamaan kuvan ja etsimään siitä nimettyä merkkiä/värikoodia.
3. Käytä `Vision.objects[index].exists` tarkistamaan että halutun kohteen merkki/värikoodi löytyy kuvassa. 

Kun kohde löytyy, niin voit käyttää muita Vision -komentoja selvittämään tarkempia tietoja kohteeta. 

* Käytä **indeksi** muuttujaa kiinnittämään kohde, josta haluat tarkempaa tietoa. Suurin esinekohde on aina edessä, jolloin se on  `Vision.objects[0]`.
* Käytä `Vision.objectCount` määrittämään motako samanlaista kohdetta löytyy halutulla merkillä/värikoodilla.
* Sitten voit käyttää muita ominaisuuksia: `angle` (kulma), `centerX` (X keskipiste), `centerY` (Y keskipiste), `height` (korkeus), `width` (leveys) and `exists` (on olemassa)

---

`Vision.objects[index].width` antaa tiedon, kuinka leveä esine on pixeleinä. Arvot ovat välillä **2 - 316 px**.

```cpp
Brain.Screen.print(MyVision.objects[1].width);
```

<advanced>
</advanced>