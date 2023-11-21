category: drive
signature: Drivetrain.setRotation(90, degrees);  
device_class: smartdrive  
description: Sets the Drivetrain's angle of rotation when configured with a VEX IQ Gyro Sensor.

# Aseta kiertokulma

Asettaa ajopelin Gyro -sensorin käännöskulman arvon.


```cpp
Drivetrain.setRotation(value, rotationUnits);
```

## Mitennkäytetään

`Drivetrain.setRotation()` komennolla ajopelin käännöskulmaksi voidaan asettaa mikä tahansa postivinen tai negatiivinen lukuarvo.

`Drivetrain.setRotation()` komento hyväksyy kokonaislukuja ja numeerisia komentoja.

`Drivetrain.setRoation()` komennolla **ei ole** rajoitusta välille 0-359 astetta.

## Esimerkki

Esimerkissä robotti kääntyy yhteensä 210 astetta:

```cpp
Drivetrain.turnToRotation(120, degrees);
Drivetrain.setRotation(-45, degrees);
Drivetrain.turnToRotation(45, degrees);
```

- Käänny vasempaan (vastapäivään) 120 astetta.
- Aseta nykyiseksi käännöskulmaksi -45 astetta.
- Käänny vasempaan (vastapäivään) 90 astetta (-45 asteesta arvoon +45 astetta) edellisen komennon perusteella.

<advanced>
</advanced>
