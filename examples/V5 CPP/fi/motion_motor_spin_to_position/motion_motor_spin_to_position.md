category: motion  
signature: MOTOR.spinToPosition(90, degrees);  
device_class: motor  
description: Spins the V5 Smart Motor to a position.  

# Pyöritä asentoon

Pyörittää V5 Älymoottorin tiettyyn asentoon.

```python 
motor.spin_to_position(POSITION, UNITS)
```

## Miten käytetään

`Motor.spinToPosition();` komento kiertää moottorin asennon haluttuun kohtaan. Perustuu nykyiseen asentoon `spin_to_position` komento kertoo mihin suuntaan pyöritään että asento saavutetaan.

Valitse mittayksikkö joko  **DEGREES** (astetta) tai **TURNS** (kierroksia).


```cpp
Motor3.spinToPosition(rotation, units);
```


**spinToPosition** komento estää toisten suorituksen kunnes V5 älymoottori on saavuttanut asennon.

## Lisäparametri

Voit valita `false` viimeiseksim parametriksi, jolloin **spinToPosition** komento ei blokkaa seuraavien komentojen suoritusta.

```cpp
Motor.spinToPosition(360, degrees, false);
```

<advanced>
</advanced>