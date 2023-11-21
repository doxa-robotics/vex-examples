category: sensing  
signature: Motor.isSpinning()  
device_class: motor  
description: Reports if the selected Motor is currently spinning.

# Moottori Pyörii

Raportoi, pyöriikö valittu moottori.

```cpp
Motor.isSpinning()
```

## Miten käytetään

Komento antaa arvon **tosi**, jos valittu moottori pyörii tällä hetkellä.

Komento antaa arvon **epätosi**, jos valittu moottori ei pyöri tällä hetkellä.

**Huomio:** Komento antaa aina arvon 'epätosi', jos moottorin pyörimiseen on annettu pelkkä `Motor.spin` -komento ilman matkaa tai astemäärää.

## Esimerkki

Esimerkissä tulostetaan vastaus VEX IQ aivojen näytölle, pyöriikö Käsimoottori.

```cpp
ArmMotor.spinFor(forward, 270, degrees, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("ArmMotor is Spinning: %s", ArmMotor.isSpinning() ? "TRUE" : "FALSE");

  // Pieni odotus ettei tulostus aiheuta sotkua
  wait(20, msec);
}
```

<advanced>
</advanced>