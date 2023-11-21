category: sensing  
signature: Drivetrain.isMoving()  
device_class: drivetrain  
description: Reports if the Drivetrain is currently moving.

# Ajopeli liikkuu?

Raportoi jos ajopeli liikkuu tällä hetkellä.

```cpp
Drivetrain.isMoving()
```

## Miten käytetään

Komento palauttaa arvon **tosi** jos ajopeli liikkuu vielä komentojen `Drivetrain.driveFor` tai `Drivetrain.turnFor` mukaan, joissa on annettu tietty matka tai astemäärä.

Komento palauttaa arvon **epätosi** jos ajopelin liike on loppunut.

**Huomio:** Komento antaa aina **epätosi** jos käytetään jatkuvia komentoja `Drivetrain.drive` tai `Drivetrain.turn` (ne *ei* määrittele ajolle tarkkaa matkaa tai kulmaa).

## Esimerkki

Esimerkissä tulostetaan tieto, liikkuuko ajopeli, VEX IQ aivojen näytölle.

```cpp
Drivetrain.driveFor(forward, 1000, mm, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain is Moving: %s", Drivetrain.isMoving() ? "TRUE" : "FALSE");

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>