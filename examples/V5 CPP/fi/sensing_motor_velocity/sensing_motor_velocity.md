category: sensing  
signature: MOTOR.velocity()  
device_class: motor  
description: Reports the current velocity of the motor.  

# Moottorin Nopeus

Raportoi valitun VEX V5 älymoottorin nopeuden.


```cpp
Motor.velocity(percent)
```

## Miten käytetään

`Motor.velocity()` palauttaa desimaalilukuna (muodossa *desimaali*) tämän hetkisen moottorin nopeuden. 

Määrittele `yksikkö`, jota komento käyttää.

**%** - palauttaa nopeuden arvon välillä **-100% - 100%**.
 
 
```cpp
Brain.Screen.print("%f", ArmMotor.velocity(percent));
```
  
`Motor.velocity()` `Motor.velocity` voi palauttaa myös arvon **rpm** (kierrosta minuutissa) riippuen vaihdepakkauksesta moottorissa seuraavasti:

**Punainen vaihdepakkaus:** -100rpm - 100rpm  
**Vihreä vaihdepakkaus:** -200rpm to 200rpm  
**Sininen vaihdepakkaus:** -600rpm to 600rpm  

```cpp
Brain.Screen.print("%f", ArmMotor.velocity(rpm));
``` 
<advanced>
</advanced>