category: drive  
signature: Drivetrain.setHeading(90, degrees);  
device_class: smartdrive  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Aseta ajosuunta

Asettaa ajopelin Gyrolle ajosuunnan arvon.

```cpp
Drivetrain.setHeading(heading, degrees);
```

## Miten käytetään

`Drivetrain.setHeading` komennolla voidaan muuttaa ajopelin nykyinen ajosuunnan arvo. 

`Drivetrain.setHeading` hyväksyy arvot väliltä **0 - 359.99** `heading` (ajosuunta) parametrille.

## Esimerkki 

Esimerkissä robotti kääntyy 135 astetta:

```cpp
Drivetrain.turnToHeading(45.0, degrees);
Drivetrain.setHeading(0.0, degrees);
Drivetrain.turnToHeading(90.0, degrees);
```
- Käänny vasempaan ajosuuntaan 45 astetta
- Aseta ajosuunnan arvoksi 0 astetta
- Käänny vasemmalle lisää 90 astetta

<advanced>
</advanced>
