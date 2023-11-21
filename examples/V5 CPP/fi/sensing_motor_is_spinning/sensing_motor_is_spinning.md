category: sensing  
signature: MOTOR.isSpinning()  
device_class: motor  
description: Reports if the selected V5 Smart Motor is currently spinning.

# Moottori pyörii

Keroo, pyöriikö V5 Älymoottori tällä hetekllä.

```cpp
Motor.isSpinning()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Komento antaa arvon **true** jos moottori pyörii , kun komennon `spinFor()` matka on vielä kesken.

Komento antaa arvon **false** jos noottorin pyörimisliike on loppunut.

**Huomio** Komento antaa aina arvon **false** jos on käytetty pelkkää `spin()` komentoa (ilman matka-arvoa).

```cpp
// esimerkissä LED valo palaa aina kun käsimoottori pyörii

ArmMotor.spinFor(forward, 720, degrees, false);

while (ArmMotor.isSpinning()) {
    LEDA.on();
    wait(0.5, seconds);
    LEDA.off();
    wait(0.5, seconds);
}
```
<advanced>
</advanced>