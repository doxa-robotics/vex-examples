category: drive  
signature: Drivetrain.turnFor(right, 90, degrees);  
device_class: drivetrain  
description: Turns the Drivetrain for a distance.  

# Käänny määrän

Kääntää ajopelin tietyn kulman haluttuun suuntaan.

```cpp
Drivetrain.turnFor(direction, angle, degrees);
```

## Miten käytetään

Aseta `direction` (suunta) ja määrä, jonka ajopeli kääntyy. Suuntavalinnat ovat **left** (vasempaan) tai **right** (oikeaan) ja määrä annetaan asteina.

```cpp
Drivetrain.turnFor(right, 270, degrees);
```

`Drivetrain.turnFor` komento blokkaa oletuksena muiden komentojen suorituksen käännöksen ajaksi.

## Lisäparametrit

Voit asettaa lisäparametriksi `false`, jos et halua että komento blokkaa oletuksena muiden komentojen suorituksen käännöksen aikana.

```cpp
Drivetrain.turnFor(left, 90, degrees, false);
```

<advanced>
</advanced>
