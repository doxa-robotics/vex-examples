category: sensing  
signature: Drivetrain.heading(degrees)  
description: Reports the Drivetrain's heading.

# Ajopelin kulkusuunta

Raportoi ajopelin kulkusuunnan.

```cpp
Drivetrain.heading(degrees)
```

## Miten käytetään

`Drivetrain.heading` raportoi kulkusuunnan arvon välillä **0.00 - 359.99 astetta**.

## Esimerkki

Esimerkissä tulostetaan ajopelin kulkusuunta VEX IQ Aivojen näytölle.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain Heading: %.2f", Drivetrain.heading(degrees));

  // Pieni odotus, ettei tulostu sotkua
  wait(20, msec);
}
```

<advanced>
</advanced>
