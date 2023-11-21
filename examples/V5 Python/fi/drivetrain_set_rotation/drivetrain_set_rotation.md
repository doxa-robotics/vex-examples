category: drivetrain
signature: drivetrain.set_rotation(0, DEGREES)  
description: Sets the Drivetrain's angle of rotation with a Gyro Sensor.

# Aseta kääntymiskulma

Asettaa ajopelin Gyro -sensorin kulman.

```don
drivetrain.set_rotation(ROTATION, UNITS)
```

## Miten käytetään

`drivetrain.set_rotation` komennolla Gyro sensorin arvoksi voi asettaa minkä tahansa positiivisen tai negatiivisen arvon.

`ROTATION` parametri sallii numeerisia arvoja.

`ROTATION` parametri ei rajoitu **does not** arvoihin 0-359 astetta.

## Esimerkki

Esimerkissä robotti kääntyy yhteensä 210 astetta:

```don
drivetrain.turn_to_rotation(120, DEGREES)
drivetrain.set_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(45, DEGREES)
```

- Käänny oikealle myötäpäivään kääntymiskulmaan 120 degrees.
- Aseta nykyinen kääntymiskulma arvoon -45 astetta.
- Käänny oikealle myötäpäivään lisää 90 astetta (-45 astetta +45 astetta) edellisen asetuksen mukaan.

<advanced>
</advanced>
