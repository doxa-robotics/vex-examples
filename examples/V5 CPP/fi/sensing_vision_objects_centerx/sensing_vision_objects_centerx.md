category: sensing  
signature: VISION.objects[0].centerX  
device_class: vision  
description: Reports the X coordinate of the center of a detected object from the Vision Sensor.

# Vision.objects[index].centerX


Antaa Vision -kameran kuvan löytämän kohteen x -akselin keskipisteen.

```cpp
Vision.objects[index].centerX
```

## Miten käytetään

Tee järjestyksessä seuraavat toimenpideaskeleet, kun käytät `Vision.objects[index]` komentoa:

1. Määrittele Vision -kamerasi Laitteet - ja Kameran määritysikkunassa.
2. Käytä `Vision.takeSnapshot()` ottamaan kuvan ja etsimään siitä nimettyä merkkiä/värikoodia.
3. Käytä `Vision.objects[index].exists` tarkistamaan että halutun kohteen merkki/värikoodi löytyy kuvassa. 

Kun kohde öytyy, niin voit käyttää muita Vision -komentoja selvittämään tarkempia tietoja kohteeta. 

* Käytä **indeksi** muuttujaa kiinnittämään kohde, josta haluat tarkempaa tietoa. Suurinesinekohde on aina edessä, jolloin se on  `Vision.objects[0]`.
* Käytä `Vision.objectCount` määrittämään motako samanlaista kohdetta löytyy halutulla merkillä/värikoodilla.
* Sitten voit käyttää muita ominaisuuksia: `angle`, `centerX`, `centerY`, `height`, `width` ja `exists`.


---
`Vision.objects[index].centerX` raportoi löydetyn kohteen keskipisteen X koordinaatin arvolla **0 - 315 px**.
```cpp
Brain.Screen.print(MyVision.objects[1].centerX);
```

---

`Vision.objects[index].centerX` raportoi löydetyn kohteen keskipisteen X koordinaatin arvolla **0 - 315 px**.
<advanced>
</advanced>