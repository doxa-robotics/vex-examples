category: drive  
signature: Drivetrain.setTimeout(1, seconds);  
device_class: drivetrain  
description: Sets the timeout for the Drivetrain to stop moving if a blocking command cannot reach its target.  

# Aseta ajoajan päättyminen

Asettaa ajopelin ajoajalle ylärajan, jos ajopeli ei saavuta muuten tavoite ajomatkaa.

```cpp
Drivetrain.setTimeout(time, seconds);
```

## Miten käytetään

`Drivetrain.setTimeout` komentoa käytetään estämään tilanne, että ohjelma päättyy kesken suorituksen ajopelin liikkumisen esteen vuoksi.

Hyvä esimerkki ajopelin liikkumisen estymisestä on, että se törmää sivuseinään eikä pysty jatkamaan asetettua tavoitematkaa.

Aseta ajoajan päättyminen ajaksi voi asettaa yksiköksi `seconds` (sekuntia).

```cpp
Drivetrain.setTimeout(2.0, seconds);
```

## Esimerkki

Esimerkissä `Drivetrain.driveFor` komento katkaisee liikkeen aika-arvoon 2 sekuntia ellei ajopeli ole ajanut tavoitematkaa 24 tuumaa. 

Kun joko aikaraja tai matka 24 tuumaa on saavutettu, ajopeli kääntyy 90 astetta oikealla.

```cpp
Drivetrain.setTimeout(2.0, seconds);
Drivetrain.driveFor(forward, 24.0, inches);
Drivetrain.turnFor(right, 90.0, degrees);
```

<advanced>
</advanced>