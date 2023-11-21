category: drive  
signature: Drivetrain.setTurnVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain when turning. If this is used when the drivetrain is turning, the drivetrain will be updated with the new speed.  

# Aseta ajopelin nopeus

Asettaa ajopelin nopeuden komennoille `drive` ja `drive_for`.

```cpp
Drivetrain.setTurnVelocity(velocity, units);
```

## Miten käytetään

`Drivetrain.setTurnVelocity();` komento asettaa ajopelin nopeuden komeentojen `drive` ja `drive_for` käyttöön. Komento ei liikuta ajopeliä.

`Drivetrain.setTurnVelocity();` hyväksyy arvoja, jotka riippuvat sen toisesta parametrista.

Jos `PERCENT` (prosenttia) on käytössä, niin nopeus **VELOCITY** hyväksyy arvot **-100 - 100**.

`Drivetrain.setTurnVelocity();` komennon **UNITS** parametrina voi käyttää `RPM` (kierrosta minuutissa). Riippuen vaihdepakkauksesta , jotka asennettu ajomoottoreihin, **VELOCITY** arvot vaihtelevat seuraavasti:

* Red Cartridge: (punainen) -100rpm to 100rpm
* Green Cartridge: Ivihreä) -200rpm to 200rpm
* Blue Cartridge: (sininen) -600rpm to 600rpm

Jos nopeudeksi asettaa negatiivisen arvon, ajopeli liikkuu vastakkaiseen suuntaa, mitä `DIRECTION` parametrissa on asetettu komennoissa `drive` tai `drive_for`.

Jos nopeus asetetaan arvoon nolla, ajopeli pysähtyy komennoilla `drive` tai `drive_for`.



<advanced>
</advanced>