category: drive  
signature: Drivetrain.setHeading(90, degrees);  
device_class: smartdrive  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Aseta ajosuunta

Asettaa ajopelin Gyrolle tarkan ajosuunnan.

```cpp
Drivetrain.setHeading(heading, degrees);
```

## Miten käytetään

`Drivetrain.setHeading();` komennolla voi ajopelin ajosuunnan muuttaa. tyypillisesti ajosuunnan arvo nollataan jossain kohtaa ohjelman suoritusta helpottamaan uuden suuunnan ottoa.

`Drivetrain.setHeading();` hyväksyy arvot välillä **0 - 360** ensimmäisenä argumenttina ja `degrees` (asteet) yksikkönä.

```cpp
// Reset the Drivetrain heading to 0

Drivetrain.setHeading(0, degrees);
```

<advanced>
</advanced>