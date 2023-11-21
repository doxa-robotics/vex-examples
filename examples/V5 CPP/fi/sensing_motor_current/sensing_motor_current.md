category: sensing  
signature: MOTOR.current()  
device_class: motor  
description: Reports the amount of current a V5 Smart Motor is currently using in amperes (amps).

# Moottorin sähkövirta

Antaa moottorin sähkövirran arvon , jota V5 älymoottori tällä hetkellä käyttää yksikössä ampeeri (amps).

```cpp
Motor.current(amp)
```

## Miten käytetään

`Motor.current()` antaa desimaaliluvun (muotoa *double*), kun se raportoi V5 älymoottori virrankulutusta tällä hetkellä käyttää.

Oletusyksikkö on ampeeri (`amp`) ja arvot mitataan välillä **0.0 - 2.5 ampeeria**.

```cpp
Brain.Screen.print("%f", ClawMotor.current(amp));
```

<advanced>
</advanced>