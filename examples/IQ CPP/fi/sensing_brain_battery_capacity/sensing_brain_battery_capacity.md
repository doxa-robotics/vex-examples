category: sensing  
signature: Brain.Battery.capacity(percent)  
description: Reports the capacity of the VEX IQ robot's battery.

# Akun lataustaso

Raportoi tämänhetkisen VEX IQ robotin akun lataustason.

```cpp
Brain.Battery.capacity(percent)
```

## Miten käytetään

`Brain.Battery.capacity` palauttaa **kokonaisluku** arvona VEX IQ robotin akun lataustason yksikkönä `%` väliltä **0 - 100**.

## Esimerkki

Esimerkissä aivojen näytölle tulostetaan VEX IQ roobotin akun lataustaso, jos se on alle 25%.

```cpp
if (Brain.Battery.capacity(percent) < 25){
  Brain.playSound(alarm);
}
```

<advanced>
</advanced>