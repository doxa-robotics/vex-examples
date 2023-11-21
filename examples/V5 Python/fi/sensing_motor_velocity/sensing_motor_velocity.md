category: sensing  
signature: motor.velocity(UNITS)
description: Reports the current velocity of a V5 Smart Motor.

# Moottorin nopeus

ANtaa nykyisen V5 Älymoottorin nopeuden.

```python
motor.velocity(UNITS)
```

## Miten käytetään

Moottorin nopesu antaa arvot väliltä **-100% - 100%** tai **-600rpm - 600rpm**.

Yksikön `UNIT` parametrit ovat: **PERCENT** (%) or **RPM** (kierrosta minuutissa).

Moottorin nopeus yksikössä "kierrosta minuutissa" arvot riippuvat käytetystä moottorin vaihdepakkauksesta.

* Red Cartridge: (punainen) -100rpm - 100rpm
* Green Cartridge: (vihreä) -200rpm - 200rpm
* Blue Cartridge: (sininen) -600rpm - 600rpm

<advanced>
</advanced>
