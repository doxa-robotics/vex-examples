category: sensing  
signature: Vision.objects  
device_class: vision  
description: Reports the objects the Vision Sensor detects. 

# Vision Kohteet

Antaa taulukon kaikista Vision -kameran havaitsemista haetuista kohteisa.

```cpp
Vision.objects
```

## Miten käytetään

Aina ensimmäisenä pitää ottaa kuva `Vision.takeSnapshot` ennen komentoa `Vision.objects` taulukkoa.

`Vision.objects` on taulukko, jossa on kuvasta kaikkien havaittujen kohteiden tiedot.

```cpp
Vision.takeSnapshot(COLOR_SIG);
vision::object firstObject = Vision.objects[0];
```
Kuvataulukkoa voi käyttää normaalin taulukon tavoin hyödyntämällä taulukon indeksejä.

```cpp
vision::object visionObject = Vision.objects[0];
```

Voit sijoittaa sen alkioita myös toistorakenteisiin esimerkiksi **Toista** komennossa `Vision.objectCount` arvoa voi käyttäää ehdoissa.

Esimerkkiohjelmasssa alla ominaisuudet `keskipisteX` and `keskipisteY` arvot tulostetaan Aivojen näytölle.

```cpp
Vision.takeSnapshot(COLOR_SIG);

for(int i = 0; i < Vision.objectCount; i++) {
  Brain.Screen.print("X: %d", Vision.objects[i].centerX);
  Brain.Screen.newLine();
  Brain.Screen.print("Y: %d", Vision.objects[i].centerY);
  Brain.Screen.newLine();
}
```

`Vision.objects` kohteet on luokkatyyppiä `vision::object` ja sillä on nämä ominaisuudet.

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