category: sensing  
signature: Drivetrain.current()  
device_class: drivetrain  
description: Reports the amount of current that the Drivetrain is currently using.

# jopelin virrankulutus

Ntaa virtamäärän jota ajoplei tällä hetkellä kuluttaa.

```cpp
Drivetrain.current(amp)
```

## Miten käytetään

`Drivetrain.current(amp)` antaa desimaaliluvun (muotoa *double*), kun sen virrankulutus mitataan.

Oletusyksikköon ampeeri (`amp`) ja arvot mitataan välillä **0.0 - 2.5 amps**.

```cpp
Brain.Screen.print("%f", Drivetrain.current(amp));
```

<advanced>
</advanced>