category: sensing  
signature: Drivetrain.isDone()  
device_class: drivetrain  
description: Reports if the Drivetrain has completed its movement.

# Ajo on suoritettu?

Raportoi onko ajopeli suorittanut liikkeen loppuun.

```cpp
Drivetrain.isDone()
```

## Miten käytetään

`Drivetrain.isDone` raportoi arvon **tosi** kun ajopelin moottorit on suorittaneet ajon loppuun.

`Drivetrain.isDone` raportoi arvon **epätosi** kun ajopelin moottorit eivät liiku.

## Esimerkki

Esimerkissä tulostetaan tieto, liikkuuko ajopelivielä vai ei, VEX IQ aivojen näytölle.

```cpp
Drivetrain.driveFor(forward, 1000, mm, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain is Done: %s", Drivetrain.isDone() ? "TRUE" : "FALSE");

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>