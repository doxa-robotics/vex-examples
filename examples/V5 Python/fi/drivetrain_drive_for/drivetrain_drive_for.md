category: drivetrain 
signature: drivetrain.drive_for(FORWARD, 2, MM, wait=True)
description: Moves the Drivetrain for a given distance.  

# Aja matka

Liikuttaa ajopeliä tietyn matkan. Kaikki ajopelin moottorit ajavat joku eteen- tai taaksepäin nopeudelle, joka on annettu komennolla `drivetrain.set_drive_velocity` . Kun matka on saavutettu, ajopeli pysähtyy.

```don
drivetrain.drive_for(DIRECTION, DISTANCE, UNITS)
```

## Miten käytetään

Kuinka pitkän matkan ajopeli liikkuu, määrätään suluissa kolmella parametrilla pilkulla eroteltuina 

Ensimmäinen argumentti on suunta 'DIRECTION' joka on joko `FORWARD` tai `REVERSE` isoilla kirjaimilla.  

Toinen argumentti on matka `DISTANCE`, jonka ajopeli ajaa.

Kolmas argumetti on 'UNITS' yksikkö , jossa matka annetaan, joko `INCHES` tai `MM` (millimetriä) isoilla kirjaimilla.

`DISTANCE` parameter accepts numeric values. Negative values will cause the V5 Robot to drive in the opposite of the input `DIRECTION`.

```
drivetrain.drive_for(REVERSE, 5.0, INCHES)
```

'drive_for` komento on ns blokkaava komento ts seuraavat komennot odottavat, että ajosuoritus on valmis.

## Lisäparametri

Voit käyttää 4. lisäparametyria `wait=False`, jolloin seuraavat komennot eivät odota ajon loppua.

```don
drivetrain.drive_for(FORWARD, 200, MM, wait=False)
```

## Esimerkki

Esimerkissä komennon `drivetrain.drive_for` matka-argumenttina on käytetty muuttujaa distance_variable.

V5 Robotti ajaa 200 MM eteenpäin.

```don
distance_variable = 200

drivetrain.drive_for(FORWARD, distance_variable, MM)
```

<advanced>
</advanced>
