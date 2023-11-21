category: sensing  
signature: Vision.takeSnapshot(signature);  
device_class: vision  
description: Takes a snapshot from the Vision Sensor. A user defined signature or color code will need to replace the "SIGNATURE" parameter in order for this example snippet to compile.

# Vision Ota kameran kuva

Ottaa Vision -kameralla kuvan.

```cpp
Vision.takeSnapshot(signature);
```

## Miten käytetään

`Vision.takeSnapshot` ottaa kuvan ja prosessoi/analysoi sen annetun Vision -kameran haetun värimerkin tiedot.

Jotta voit ottaa `Vision.takeSnapshot` komennon, Vision -kameralle pitää olla määritelty ainakin yksi esine/värimerkki. Värimerkin oletusnimi on automaattisesti määritelty.

Esimerkissä Vision -kameran nimi on `Vision1` ja värimerkin `REDBOX`, valittu kokonimi on `Vision1__REDBOX` ja jos haluat ottaa kuvan ko. värimerkillä valitse komento:

```cpp
Vision1.takeSnapshot(Vision1__REDBOX);
```

Tyypillisesti aina ensimmäinen Vision -komento on `Vision.takeSnapshot` ennen muita Vision -kamerakomentoja.

Muista tarkentaa Vision -merkki (esine jota haet).Merkit määritellään ensin Kameran määritys-ikkunassa.

<advanced>
</advanced>