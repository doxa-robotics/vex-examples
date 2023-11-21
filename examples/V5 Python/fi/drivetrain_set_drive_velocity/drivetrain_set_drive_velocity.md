category: drivetrain  
signature: drivetrain.set_drive_velocity(VELOCITY, PRECENT)  
description: Sets the velocity of the Drivetrain that will be used for drive() and drive_for() commands.

# Aseta ajopelin nopeus

Asettaa ajopelin nopeuden komennoille `drive` ja `drive_for`.

```python
drivetrain.set_drive_velocity(VELOCITY, UNITS)
```

## Miten käytetään

`drivetrain.set_drive_velocity` komento asettaa ajopelin nopeuden komeentojen `drive` ja `drive_for` käyttöön. Komento ei liikuta ajopeliä.

`drivetrain.set_drive_velocity` hyväksyy arvoja, jotka riippuvat sen toisesta parametrista.

Jos `PERCENT` (prosenttia) on käytössä, niin nopeus **VELOCITY** hyväksyy arvot **-100 - 100**.

`drivetrain.set_drive_velocity` komennon **UNITS** parametrina voi käyttää `RPM` (kierrosta minuutissa). Riippuen vaihdepakkauksesta , jotka asennettu ajomoottoreihin, **VELOCITY** arvot vaihtelevat seuraavasti:

* Red Cartridge: (punainen) -100rpm to 100rpm
* Green Cartridge: Ivihreä) -200rpm to 200rpm
* Blue Cartridge: (sininen) -600rpm to 600rpm

Jos nopeudeksi asettaa negatiivisen arvon, ajopeli liikkuu vastakkaiseen suuntaa, mitä `DIRECTION` parametrissa on asetettu komennoissa `drive` tai `drive_for`.

Jos nopeus asetetaan arvoon nolla, ajopeli pysähtyy komennoilla `drive` tai `drive_for`.

## Esimerkki

Esimerkissä Drivetrain ajaa taaksepäin, kun nopeus määrätty negatiivisella luvulla.

```python
drivetrain.set_drive_velocity(-100, PERCENT)
drivetrain.drive(FORWARD)
```

Tässä ajopeli ei liiku

```python
drivetrain.set_drive_velocity(0, PERCENT)
drivetrain.drive(FORWARD)
```

<advanced>
</advanced>
