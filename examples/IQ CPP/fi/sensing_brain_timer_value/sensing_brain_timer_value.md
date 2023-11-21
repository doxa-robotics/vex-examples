category: sensing  
signature: sensing_brain_timer_value
description: Reports the VEX IQ Brain's timer value in seconds. 

# Kello

Raportoi VEX IQ Aivojen kellon ajankulun sekunteina.

```cpp
Brain.Timer.value()
```

## Miten käytetään

Aivojen kello lähtee liikkeelle arvosta 0, kun ohjelma käynnistyy ja palauttaa arvon desimaalilukuna (*double*).

## Esimerkki

Esimerkissä tulostaan aivojen kellon aika.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Timer: %.2f", Brain.Timer.value());
  
  // Pieni odotus estää päällekkäisen tulostuksen sotkun
  wait(20, msec);
}
```

<advanced>
</advanced>