category: sensing  
signature: Drivetrain.isDone()  
device_class: drivetrain  
description: Reports if the Drivetrain has completed its movement.

# Ajopeli on pysähtynyt

Antaa tiedon onko ajopeli lopettanut liikkeensä.

```cpp
Drivetrain.isDone()
```

## Miten käytetään

Komennot, jotka palauttavat arvon voidaan sijoittaa toisten komentojen sisään kuten print -komennossa tao ohjauslauseissa ehtomuuttujien osana ja ilman puolipistettä.

`Drivetrain.isDone()` antaa arvon **true** jos ajopeli on pysähtynyt ts suorittanut liikeensä loppuun.

`Drivetrain.isDone()` antaa arvon **false** jos ajopeli on liikeessä vielä.

```cpp
waitUntil(Drivetrain.isDone());
```

Komento antaa arvon **true** jos kyseessä on komennojen `drive()` tai `turn()` tarkastelu.

<advanced>
</advanced>