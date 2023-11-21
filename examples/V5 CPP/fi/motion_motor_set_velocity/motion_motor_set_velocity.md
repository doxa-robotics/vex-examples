category: motion  
signature: MOTOR.setVelocity(50, percent);  
device_class: motor  
description: Sets the V5 Motor's velocity.  

# Asettaa moottorin nopeuden

Asettaa V5 Älymoottorille nopeusarvon pyörimiseen.

```cpp
Motor.setVelocity(velocity, units);
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



<advanced>
</advanced>