category: control  
signature: control_if_else
description: Runs the code inside the else-statement's curly brackets, if the if-statement's condition is false. This command must have an if-statement preceding for it to compile.  

# Jos niin muuten

Ohjaislauseen ensimmäisen tai toisen aaltosulun sisällä olevat komennot suoritetaan riippuen ehdon Boolean arvosta.

```cpp
if (condition) {
  // Koodi joka suoritettan tosi tilanteessa
} else {
  // Kood, joka suoritetaan epätosi tilanteessa
}
```

## Miten käytetään

Jos niin muuten -komento tutkii vain Boolean ehtoa kerran.

Jos Boolean `(condition)` ehto on tosi **true**, suoritetaan Jos -haara.

Jos Boolean `(condition)` ehto on epätosi **false**, suoritetaan Muuten -haara.

## Esimerkki

Esimerkissä VEX IQ KosketusLED loistaa vihreää, kun sitä on painettu, muuten se loistaa punaista kun sitä ei ole painettu.

Jos muuten -ehdon voi laittaa jatkuvaan toistorakenteeseen upotettuna nestedâ, jolloin ledilampun valoa voidaan muuttaa useamman kerran.

```cpp
while (true) {
  if (TouchLED.pressing()) {
    TouchLED.setColor(green);
  } else {
    TouchLED.setColor(red);
  }

  wait(20, msec);
}
```

<advanced>
</advanced>