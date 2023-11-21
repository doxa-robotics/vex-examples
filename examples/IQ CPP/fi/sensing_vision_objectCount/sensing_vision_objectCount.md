category: sensing  
signature: Vision.objectCount  
device_class: vision  
description: Reports how many objects the Vision Sensor detects. 

# Vision Kohteiden lukumäärä

raportoi monta haettua kohdetta Vision -kamera havaitsee kuvassa. 

```cpp
Vision.objectCount
```

## Miten käytetään

Määrittele Vision -kamera käyttöön Laitteet-ikkunassa

Määrittele merkit/värikoodit Kameran määritysikkunassa. 

Ota kuva `Vision.takeSnapshot` halutulla merkillä/värikoodilla .

`Vision.objectCount` antaa viimeisimmästä kuvasta havaittujen kohteiden lukumäärän.

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