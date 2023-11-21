category: motion  
signature: motor.set_velocity(VELOCITY, UNITS)  
description: Sets the speed of a V5 Smart Motor.

# Asettaa moottorin nopeuden

Asettaa V5 Älymoottorille nopeusarvon pyörimiseen.

```don 
motor.set_velocity(VELOCITY, UNITS)
```

## Miten käytetään

Komento hyväksyy arvot välillä **-100% to 100%** tai **-600rpm to 600rpm.**

Hyväksytyt `UNITS` parametrit ovat joko `PERCENT` (%) or `RPM`.

**Set motor velocity** hyväksyy  "rotations per minute" (RPM) arvot riippuen käytetystä vaihdepakkauksesta V5 Älymoottorissa.

* Red Cartridge: (punainen) -100rpm to 100rpm
* Green Cartridge: (Vihreä) -200rpm to 200rpm
* Blue Cartridge: (Sininen) -600rpm to 600rpm

Jos nopeuden asettaa negatiivisen arvon, moottori pyörii taaksepäin (vastapäivään).

Moottorin saa pysäyhtymään, kun asettaa sille nopeusarvon 0.

## Esimerkki

Esimerkissä moottorin nopeus asetaan arvoon 25% ja moottori pyörii asentoon 90 astetta.

```don
arm_motor.set_velocity(25, PERCENT)
arm_motor.spin_to_position(90, DEGREES)
```

<advanced>
</advanced>
