category: sensing  
signature: VISION.objectCount  
device_class: vision  
description: Reports how many objects the Vision Sensor detects. 

# Vision Kohteiden lukumäärä

Raportoi montako haettua kohdetta Vision -kamera havaitsee kuvassa. 


An object will need to be configured before the `Vision.objectCount` command can detect it.

```cpp
Vision.objectCount
```

## Miten käytetään

Määrittele Vision -kamera käyttöön Laitteet-ikkunassa

Määrittele merkit/värikoodit Kameran määritysikkunassa. 

Ota kuva `Vision.takeSnapshot` halutulla merkillä/värikoodilla .

`Vision.objectCount` antaa viimeisimmästä kuvasta havaittujen kohteiden lukumäärän.

```cpp
Vision.objectCount
```
## Esimerkki

Esimerkissä tulostetaan aivojen näytölle viimeisimmän kuvan havaittujen kohteiden lukumäärä.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);

  // Ota kuva merkillä SIGNATURE
  Vision.takeSnapshot(SIGNATURE);

  Brain.Screen.print("Number of Objects Detected: %d", Vision.objectCount);

  // Ota kuva joka 20 millisekuntia
  wait(20, msec);
}
```

<advanced>
</advanced>