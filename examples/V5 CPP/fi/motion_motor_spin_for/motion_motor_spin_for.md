category: motion  
signature: MOTOR.spinFor(forward, 90, degrees);  
device_class: motor  
description: Spins the V5 Smart Motor for distance.  

# Pyöri matka
 
Komento pyörittää V5 älymoottoria tietyn matkan joko asteina tai kierroksina.


```cpp
Motor.spinFor(directionType, rotation, units);
```

## How To Use

`Motor.spinFor();` Valitse suunta `DIRECTION` , johon moottori pyörii: **FORWARD** (eteenpäin) tai **REVERSE** (taaksepäin).

The `Motor.spinFor();` hyväksyy numeerisen arvon parametriin `rotation`.

Valitse mittayksikkö `UNIT` joko **DEGREES** (astetta) tai **TURNS** (kierroksia).

**spinFor** komento blokkaa seuraavat komennot suorituksen ajaksia oletuksena.

## Lisäparametri

Valitse lisäparametri `false` kun  **spinFor** jälkeen seuraava komento suoritetaan ilman odotusta.

```cpp
Motor.spinFor(forward, 360, degrees, false);
```
<advanced>
</advanced>
