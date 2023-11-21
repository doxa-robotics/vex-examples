category: sensing  
signature: Drivetrain.power()  
device_class: drivetrain  
description: Reports the amount of power output the Drivetrain is currently generating.

# Ajopelin teho

ANtaa ajopelin moottoreiden tehomäärän.

```cpp
Drivetrain.power()
```

## Miten käytetään

`Drivetrain.power()` antaa desimaaliluvun (muotoa *double*) ajopelin kehottämän tehon määrälle.

Komennot, jotka palauttavat arvon voidaan sijoittaa toisten komentojen sisään kuten print -komennossa tao ohjauslauseissa ehtomuuttujien osana ja ilman puolipistettä.

Oletusyksikkö on `watt` ja arvot ovat välillä **0.0 - 22.0 wattia**. 


```cpp
Brain.Screen.print("%f", Drivetrain.power());
```
<advanced>
</advanced>