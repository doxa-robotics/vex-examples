category: drive  
signature: Drivetrain.setHeading(90, degrees);  
device_class: smartdrive  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Aseta ajopelin kääntymiskulma

Asettaa ajopelin kääntymiskulmalle uuden arvon VEX IQ Gyro Sensorissa.

```cpp
Drivetrain.setRotation(rotation, degrees);
```
## Miten käytetään

`Drivetrain.setRotation` komennolla voi ajopelin kääntymiskulmaa asettaa mihin postiiviseen tai negatiiviseen kääntymiskulmaan haluaa.

## Esimerkki

Esimerkissä robotti kääntyy 210 astetta:

```cpp
Drivetrain.turnToRotation(120, degrees);
Drivetrain.setRotation(-45, degrees);
Drivetrain.turnToRotation(45, degrees);
```

- Käänny vasemmalle (vastapäivään) suuntaan 120 astetta.
- Aseta robotin nykyinen kääntymiskulma arvoon -45 asetta.
- Käänny vasemmalle (vastapäivään) lisää suuntaan 45 astetta (-45 degrees to +45 degrees).

<advanced>
</advanced>