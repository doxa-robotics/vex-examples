category: drivetrain 
signature: drivetrain.turn_to_heading(90, DEGREES)  
description: Turns a Drivetrain to a specific heading, when using the Gyro or Inertial sensors.

# Käänny ajosuuntaan

Kääntää ajopeliä tiettyyn ajosuuntaan sen Gyro tai Inertial sensorin avulla.

`drivetrain.turn_to_heading(HEADING, UNITS)`

## Miten käytetään

`drivetrain.turn_to_heading` komentoa käytetään kääntämään ajopeliä halutuun kellotaulun ajosuuntaan.

Komento perustuu nykyiseen Gyron ajosuuntaan ja `drivetrain.turn_to_heading` määrittää tämän mukaan mihin suuntaan käännös tehdään.

`HEADING` parametri hyväksyy arvot välillä **0.00 - 359.99** .

Yksikkö `UNITS` parametri on asteita `DEGREES`.

## Esimerkki

Esimerkissä ajopeli tekee neljä käännöstä: 

```don
drivetrain.turn_to_heading(45.0, DEGREES)
drivetrain.turn_to_heading(90.0, DEGREES)
drivetrain.turn_to_heading(270.0, DEGREES)
drivetrain.turn_to_heading(180.0, DEGREES)
```

- oikealla ajosuuntaan 45 astetta
- oikealle ajosuuntaan 90 astetta
- Oikealle ajosuuntaan 270 astetta
- Vasemmalle ajosuuntaan 180 astetta

`turn_to_heading` kometo estää/odottaa seuraavien kometojen suorituksen kunnes se on saanut käännöäksen valmiiksi.

## Lisäparametrit

Voit käyttää parametria `wait=False` kolmantena parametrina, jos haluat jatkaa suoraan `turn_to_heading` komennon jälkeiseen komentoon odottamatta ajopelin käännöstä loppuun.

```don
drivetrain.turn_to_heading(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
