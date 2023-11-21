category: sensing  
signature: Bumper.pressing()  
device-class: bumper
description: Reports if the VEX IQ Bumper is pressed.

# Painokytkintä Painettu

Raportoi, onko painokytkintä painettu.

```cpp
Bumper.pressing()
```

## Miten käytetään

`Bumper.pressing` raportoi arvon **tosi**, kun painokytkintä on painettu.

`Bumper.pressing` raportoi arvon **epätosi**, kun painokytkintä ei ole painettu.

Komennon ensimmäinen osa on nimetty painokytkin.

```cpp
Bumper2.pressing()
Bumper4.pressing()
```

## Esimerkki

Esimerkissä aivojen näytölle tulostetaan, onko painokytkintä painettu ai ei.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Bumper Pressed: %s", Bumper2.pressing() ? "TRUE" : "FALSE");

  // Pieno odotus, ettei tulostu sotkua
  wait(20, msec);
}
```

<advanced>
</advanced>
