category: drive  
signature: Drivetrain.driveFor(forward, 200, mm);  
device_class: drivetrain  
description: Moves the Drivetrain for a given distance.  

# Aja matka

Liikuttaa ajopeliä tietyn matkan. Kaikki ajopelin moottorit ajavat joku eteen- tai taaksepäin nopeudelle, joka on annettu komennolla `Drivetrain.setDriveVelocity` . Kun matka on saavutettu, ajopeli pysähtyy.

```cpp
Drivetrain.driveFor(directionType, distance, distanceUnits);
```

## Miten käytetään

Anna ajosuunta (`forward` tai `reverse`) ja ajomatka yksikössä (`inches` tai `mm`).

`Drivetrain.driveFor();` komento hyväksyy numeerisia arvoja matkaarvoon `distance`.

```cpp
Drivetrain.driveFor(reverse, 5.0, inches);
```

**driveFor** komento estää muiden komentojen suorituksen kunnes matka on suoritettu.

## Lisäparamtri

Voit asettaa arvon `false` viimeiselle parametrille, jolloin **driveFor** komento ei estä seuraavia komentoja matkan ollessa kesken.

```cpp
Drivetrain.driveFor(forward, 5.0, inches, false);
```

<advanced>
</advanced>
