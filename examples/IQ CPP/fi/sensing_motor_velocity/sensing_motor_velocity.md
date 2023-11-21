category: sensing  
signature: Motor.velocity(units)  
device_class: motor  
description: Reports the current velocity of the motor.  

# Moottorin Nopeus

Raportoi valitun VEX IQ älymoottorin nopeuden.

```cpp
Motor.velocity(units)
```

## Miten käytetään

`Motor.velocity` palauttaa desimaalilukuna (muodossa *desimaali*) tämänhetkisen moottorin nopeuden. 

Määrittele `yksikkö`, kun komentoa käytetään.

**%** - palauttaa nopeuden arvon välillä **-100% - 100%**.
 
```cpp
Brain.Screen.print("%f", Motor.velocity(percent));
```
  
`Motor.velocity` voi palauttaa myös arvon **rpm** (kierrosta minuutissa).

```cpp
Brain.Screen.print("%f", Motor.velocity(rpm));
``` 

<advanced>
</advanced>