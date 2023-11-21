category: control  
signature: control_break
description: Exits a repeating loop immediately.

# Keskeytä

Hyvätään toistorakmneteen sisältä.

```cpp
break;
```

## Miten käytetään

Kun asetaa luupin sisälle `break` komennon, niin loopista tehdään hyppy pois exit heti. 

## Esimerkki

esimerkissäe ajopeli liikkuu eteenpäin ja tutkitaan onko  VEX IQ aivojen Ylös-painiketta on painettu.

Heti jos Ylös-painiketta on painettu poistutaan 'while' luupista ja ajopeli pysähtyy.

```cpp
while (true) {
  Drivetrain.drive(forward);
  if (Brain.buttonUp.pressing()) {
    break;
  }
  wait(20, msec);
}

Drivetrain.stop();
```
<advanced>
</advanced>
