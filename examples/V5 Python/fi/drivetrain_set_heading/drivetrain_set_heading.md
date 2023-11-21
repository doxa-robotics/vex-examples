category: drivetrain
signature: drivetrain.set_heading(0, DEGREES)  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Aseta ajosuunta

Asettaa ajopelin Gyrolle tarkan ajosuunnan.

```don
drivetrain.set_heading(HEADING, UNITS)
```

## Miten käytetään

`drivetrain.set_heading` komennolla voi ajopelin ajosuunnan muuttaa. tyypillisesti ajosuunnan arvo nollataan jossain kohtaa ohjelman suoritusta helpottamaan uuden suuunnan ottoa.

`drivetrain.set_heading` hyväksyy arvot välillä **0 - 360** ensimmäisenä argumenttina ja `DEGREES` (asteet) kirjoitettuna isoilla kirjaimilla.

## Esimerkki

Esimerkissä ajosuunta asetetaan arvoon 90 astetta. 

Koska ajosuunta on asetettu arvoon 90 astetta, ei seuraava komento `turn_to_heading` muuta asentoa, koska se on sama asetuksen mukainen.

```don
drivetrain.set_heading(90, DEGREES)
drivetrain.turn_to_heading(90, DEGREES)
```

<advanced>
</advanced>
