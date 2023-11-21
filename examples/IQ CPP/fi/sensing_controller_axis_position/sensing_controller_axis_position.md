category: sensing  
signature: Controller.Axis.position()  
device_class: controller  
description: Reports the position of a joystick on the IQ Controller along an axis.  

# Ohjain Tatin Asento

Raportoi valitun ohjaimen tatin asennon akselillaan.

```cpp
Controller.Axis.position()
```

## Miten käytetään

`Controller.Axis.position` antaa arvot välillä **-100 - 100**.

`Controller.Axis.position` antaa arvon **0**, kun tatin asento on keskellä.

Valitse tatti, jota seurataan.

* `AxisA` - vasen tatti (ylös ja alas)
* `AxisB` - vasen tatti vasempaan ja oikeaan)
* `AxisC` - oikea tatti vasempaan ja oikeaan)
* `AxisD` - oikea tatti (ylös ja alas)

## Esimerkki

Esimerkissä tulostetaan Aivojen näytölle ohjaimen tatin A (AxisA) arvo.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("AxisA Position: %.0f", Controller.AxisA.position());

  // Pieni odotus,ette näytölle tulostu sotkua
  wait(20, msec);
}

```

<advanced>
</advanced>