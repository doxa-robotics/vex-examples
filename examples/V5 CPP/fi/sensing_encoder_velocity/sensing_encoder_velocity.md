category: sensing  
signature: ENCODER.velocity(dps)  
device_class: encoder  
description: Reports the current velocity of a Shaft Encoder.

# Encoder Nopeus

Antaa akseli kiertomittarin / Encoderin nopeuden.

```cpp
Encoder.velocity(units)
```

## Miten käytetään

`Encoder.velocity()` antaa desimaaliluvun (muotoa *double*) joku asteina per sekuntti (`dps`) tai kierroksia minuutissa (`rpm`).


Arvot yksikössä astetta minuutissa (`dps`).

```cpp
Brain.Screen.print("%f", EncoderC.velocity(dps));
```

Arvot yksikössä kierrosta minuutissa (`rpm`).

```cpp
Brain.Screen.print("%f", EncoderC.velocity(rpm));
```
<advanced>
</advanced>