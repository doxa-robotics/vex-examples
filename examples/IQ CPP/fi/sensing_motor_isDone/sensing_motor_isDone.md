category: sensing  
signature: Motor.isDone()  
device_class: motor  
description: Reports if the Motor has completed its movement.

# Mooottori on pysähtynyt?

raportoi onko moottori suorittanut loppuun liikkeensä.

```cpp
Motor.isDone()
```

## Miten käytetään

`Motor.isDone` antaa arvon **tosi**, kun tietty moottori on pysähtynyt.

`Motor.isDone` antaa arvon **epätosi**, kun tietty moottori ei ole suorittanut liikettä loppuun.

## Esimerkki

Esimerkissä tulostetan aivojen näytölle tiedot, onko käsimoottori suorittanut pyörimisen loppuun.

```cpp
ArmMotor.spinFor(forward, 270, degrees, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("ArmMotor is Done: %s", ArmMotor.isDone() ? "TRUE" : "FALSE");

  // Pieni odotus, ettei tulostus aiheuta sotkua
  wait(20, msec);
}
```

<advanced>
</advanced>