category: drive
signature: Drivetrain.setRotation(90, degrees);  
device_class: smartdrive  
description: Sets the Drivetrain's angle of rotation when configured with a 3-Wire Gyro Sensor or V5 Inertial Sensor.

# Aseta kääntymiskulma

Asettaa ajopelin Gyro -sensorin kulman.

```cpp
Drivetrain.setRotation(rotation, degrees);
```

## Miten käytetään

`Drivetrain.setRotation()` komennolla Gyro -sensorin arvoksi voi asettaa minkä tahansa positiivisen tai negatiivisen arvon.

`Drivetrain.setRotation()` sallii numeerisia arvoja.

`Drivetrain.setRotation()` ei rajoitu **does not** arvoihin 0-359 astetta.

## Esimerkki

esimerkissä robotti kääntyy yhteensä 210 astetta:

```cpp
Drivetrain.turnToRotation(120, degrees);
Drivetrain.setRotation(-45, degrees);
Drivetrain.turnToRotation(45, degrees);
```
Käänny oikealle myötäpäivään lisää 90 astetta (-45 astetta +45 astetta) edellisen asetuksen mukaan.

- Käänny oikealla myötäpäivään kääntymiskulmaan 120 degrees.
- Aseta nykyinen kääntymiskulma arvoon -45 astetta.
- Käänny oikealle myötäpäivään lisää 90 astetta (-45 astetta +45 astetta) edellisen asetuksen mukaan.

<advanced>
</advanced>
