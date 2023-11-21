category: sensing  
signature: Vision.largestObject  
description: Reports the largest object that the vision sensor sees.

# Vision Suurin Kohde

Palauttaa Kameran kuvasta havaituista kohteista suurimman kohteen tiedot.

```cpp
Vision.largestObject
```

## Miten käytetään

Ota kuva `Vision.takeSnapshot` ennenkuin voit käyttää suurimman kohteen tietoja `Vision.largestObject` komennolla.

`Vision.largestObject` suurimman kohteen komento on luokkatyyppiä `vision::object`.

```cpp
// Ota kuva merkillä COLOR_SIG 
Vision.takeSnapshot(COLOR_SIG);

Brain.Screen.print("X: %d", Vision.largestObject.centerX);
Brain.Screen.newLine();
Brain.Screen.print("Y: %d", Vision.largestObject.centerY);
Brain.Screen.newLine();
```

`Vision.largestObject` on luokkatyyppiä `vision::object` , jolla on seuraavat ominaisuudet.

- `id`      - Kohteen yksikäsitteinen ID numero , on tyyppiä `int`
- `originX` - Kohten vasen yläkulma X -akselilla, on tyyppiä `int`
- `originY` - kohteen vasen yläkulma Y -akselilla, on tyyppiä `int`
- `centerX` - Kohteen Keskipiste X-akselilla on tyyppiä `int`
- `centerY` - Kohteen keskipiste Y -akselilla on tyyppiä `int`
- `width`   - Kohteen leveys on tyyyppiä `int`
- `height`  - Kohteen korkeus on tyyppiä `int`
- `angle`   - Kohteen muodostama kulma kameraan on tyyppiä `double`
- `exists`  - Jos kohde löytyy on tyyppiä `bool`

<advanced>
</advanced>