category: drive  
signature: Drivetrain.driveFor(forward, 1, inches);  
device_class: drivetrain  
description: Moves the Drivetrain for a given distance.  

# Aja matka

Liikuttaa ajopeliä tietyn matkan. 

```cpp
Drivetrain.driveFor(direction, distance, units);
```

## Miten käytetään

Valitse `direction` (suunta), johon ajopeli liikkuu - joko **forward** (eteenpäin) tai **reverse** (taaksepäin). 

Aseta matka, jonka ajopeli liikkuu numeerisen arvona parametrissa `distance` (matka). 

Valise 'units' yksiköksi joko **inches** (tuumaa) tai **mm**.

```cpp
Drivetrain.driveFor(reverse, 5, inches);
```

`Drivetrain.driveFor` oletuksena blokkaa seuraavien komentojen suorituksen matkan ajaksi.

## Lisäparametrit

Voit asetaa viimeiseksi parametriksi `false` (epätosi), jolloin `Drivetrain.driveFor` komento ei blokkaa seuraavien komentojen suoritusta matkan ajaksi.

```cpp
Drivetrain.driveFor(forward, 200, mm, false);
```

<advanced>
</advanced>
