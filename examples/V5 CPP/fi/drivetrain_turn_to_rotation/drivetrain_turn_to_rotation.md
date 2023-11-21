category: drive 
signature: Drivetrain.turnToRotation(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific angle of rotation when configured with a 3-Wire Gyro Sensor or V5 Inertial Sensor.  

# Käännä kiertokulmaa määrän

Kääntää ajopeliä kiertokulman tiettyyn astemäärään nykyisen gyron astemäärän perusteella.

`Drivetrain.turnToRotation(rotation, units);`

## Miten käytetään

`Drivetrain.turnToRotation();` komentoa voi käyttää kääntämään ajopeliä positiivisen arvolla myötäpäivään tai negatiivisella arvolla vastapäivään.

Riippuen nykyisestä kääntymiskulman arvosta gyrosensorissa `Drivetrain.turnToRotation();` päättelee mihin suuntaan se kääntyy.

`ROTATION` parametri hyväksyy numeerisia rvoja.

Numeeriset arvot eivät **not** rajoita arvoja välillä **0 - 359.99** astetta. Käännökset ovat absoluuttisia ja voivat kääntää robottia enemmän kuin kerran

## Esimerkki

Esimerkissä ajopeli tekee 4 käännöstä:
```cpp
Drivetrain.turnToRotation(90.0, degrees);
Drivetrain.turnToRotation(180, degrees);
Drivetrain.turnTorotation(-45, degrees);
Drivetrain.turnToRotation(0, degrees);
```


- Oikealla myötäpäivään kohtaan 90 astetta
- Oikealla myötäpäivään kohtaan 180 astetta
- Vasemmalle vastapäivään kohtaan -45 astetta
- Oikealla myötäpäivään kohtaan 0 astetta

`Drivetrain.turnToRotation();` komento estää muita komentojen suorituksen , jos käännös on kesken.

## Lisäparametri 

Voit lisä paremetrin `wait=False`, jolloin `Drivetrain.turnToRotation();` komento ei estä seuraavien komentojen suoritukset kesken käännöstä.

```cpp
Drivetrain.turnToRotation(180.0, degrees, false);
```

<advanced>
</advanced>