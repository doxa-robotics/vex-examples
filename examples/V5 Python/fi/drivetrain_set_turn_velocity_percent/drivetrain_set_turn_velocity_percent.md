category: drivetrain
signature: drivetrain.set_turn_velocity(VELOCITY, PERCENT)  
description: Sets the Drivetrain's turn velocity.

# Aseta kääntymisnopeus

Asettaa ajopelin kääntymisen nopeuden.

```python
drivetrain.set_turn_velocity(VELOCITY, UNITS)
```

## Miten käytetään

`drivetrain.set_turn_velocity` asettaa ajopelin kääntymisnopeuden, mutta se ei liikuta ajopeliä. Nopeus asetetaan kääntymiskomennoille `turn` tai `turn_for`.

`drivetrain.set_turn_velocity` hyväksyy arvoja, jotka riippuvat yksiköstää, jota käytetään toisessa parametrissa.

Jos `PERCENT` (prosentti) yksikkö on käytössä toisena parametrina, arvot voivat olla välillä **-100 - 100**.

vaihtoehtoisesti `drivetrain.set_turn_velocity` komennon  toinen parametri **UNITS** voi olla `RPM`. Riippuen asennetuista vaihdepakkauksista ajomoottoreihin **VELOCITY** parametrin arvot voivat olla välillä:

* Red Cartridge: (punainen) -100rpm to 100rpm
* Green Cartridge: (vihreä) -200rpm to 200rpm
* Blue Cartridge: (sininen) -600rpm to 600rpm

Jos asettaa ajopelin kääntymisnopeuden negatiiviseena rvoon, ajopeli liikkuu oletetsesta vastakkaiseen suuntaan.

Jos asettaa ajopelin kääntymisnopeuden arvoon nolla, niin ajopeli pysähtyy komermmoilla `turn` ja `turn_for`.

## Esimerkki

Esimerkissä ajopeli kääntyy vastakkaiseen suuuntaan vasemmalle , kun kääntymisnopeus on asetettu negatiiviseen arvoon.

```python
drivetrain.set_turn_velocity(-100, PERCENT)
drivetrain.turn(RIGHT)
```

<advanced>
</advanced>
