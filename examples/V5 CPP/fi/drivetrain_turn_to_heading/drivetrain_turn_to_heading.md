category: drive  
signature: Drivetrain.turnToHeading(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific heading, when using the Gyro or Inertial sensors.

# AJopelin kääntyminen ajosuuntaan

Kääntää ajopelin tiettyyn ajosuuntaanhen Gyro tai Inertial sensorin avulla.

`Drivetrain.turnToHeading(heading, units);`

## Miten käytetään

`Drivetrain.turnToHeading();` komennolla saadaan ajopeli kääntymään mihin tahansa myötäpäivään ajosuuntan.

Pohjautuu nykyiseen Gyron ajosuuntaan, `Drivetrain.turnToHeading();` päättelee kääntymissuunnan.

`Drivetrain.turnToHeading();` hyväksyy arvot välillä **0.00 - 359.99**, kun yksikö on asteita `degrees`.

## Esimerkki

Esimerkissä ajopeli tekee neljä käännöstä: 

```cpp
Drivetrain.turnToHeading(45.0, degrees);
Drivetrain.turnToHeading(90.0, degrees);
Drivetrain.turnToHeading(270.0, degrees);
Drivetrain.turnToHeading(180.0, degrees);
```

- Oikealle suuntaan 45 astetta
- Oikealle suuntaan 90 astetta
- Oikealle suuntaan 270 astetta
- vasemmalle suuntaan 180 astetta

**turnToHeading** estää seuraavien komentojen suorituksen kääntymisen ajan.

## Lisäparametri

Kun asetat arvon `false` lisäparametrille **turnToHeading** komennolle niin kääntyminesen jälkeinen komento suoritetaan heti.

```cpp
Drivetrain.turnToHeading(180.0, degrees, false);
```

<advanced>
</advanced>