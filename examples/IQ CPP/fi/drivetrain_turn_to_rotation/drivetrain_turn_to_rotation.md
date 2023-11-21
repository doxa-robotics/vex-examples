category: drive 
signature: Drivetrain.turnToRotation(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific angle of rotation when configured with a VEX IQ Gyro Sensor.

# Käännä kiertokulmaa

Kääntää ajopelin kiertokulmaa VEX IQ Gyro Sensorin avulla.

```cpp
Drivetrain.turnToRotation(rotation, degrees);
```

## Miten käytetään

`Drivetrain.turnToRotation` komentoa voi käyttää kääntämään ajopeliä tiettyyn asentoon , positiiviseen (vastapäivään) tai negatiiviseen (myötäpäivään) arvoon.

Perustuu ajopelin nykyiselle kääntymiskulmalle, `Drivetrain.turnToRotation` määrittää mihin suuntaan käännytään.

`Kääntymis` parametri **ei** ole rajattu arvoihin välillä **0 - 359.99 astetta**. Käännös on absoluuttinen ja kääntää robottia useammin kuin kerran jos tarvis.

## Esimerkki

Esimerkissä ajopeli tekee 4 käännöstä:

```cpp
Drivetrain.turnToRotation(90.0, degrees);
Drivetrain.turnToRotation(180, degrees);
Drivetrain.turnToRotation(-45, degrees);
Drivetrain.turnToRotation(0, degrees);
```

- Vasempaan (vastapäivään) kiertokulmaa 90 astetta
- Vasempaan (vastapäivään) kiertokulmaa 180 astetta
- Oikealle (myötäpäivään) kiertokulmaa -45 astetta
- vasemmalle (vastapäivään) kiertokulmaa 0 astetta

`Drivetrain.turnToRotation`komento blokkaa seuraavat komennot kunnes käännös on suoritettu.

## Lisäparametrit

Voi asettaa lisäparametrin arvon `false`, jolloin `Drivetrain.turnToRotation();` seuraava komento ei odota liikkeen loppumista.

```cpp
Drivetrain.turnToRotation(180.0, degrees, false);
```

<advanced>
</advanced>
