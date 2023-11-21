category: sensing  
signature: drivetrain.velocity(UNITS)
description: Reports the current velocity of the Drivetrain.

# Ajopelin nopeus
 
Antaa ajopelin nykyisen nopeuden.

```python
drivetrain.velocity(UNITS)
```

## Miten käytetään

`drivetrain.velocity` palauttaa desimaalilukuna ajopelin nykyisen nopeuden.

Yksikkö `UNITS` voi olla joko **PERCENT** (prosenttia) tai **RPM** (kierrosta minuutissa)..

Jos käytetään yksikön `UNITS` parametrina **PERCENT**, arvot saadaan väliltä **-100% - 100%**.

Vastaavasti jos yksikön `UNITS` parametrina on **RPM**, mitatut arvot riippuvat asennetuista moottorien vaihdelaatikoiden väreistä seuraavasti.

* Red Cartridge: (punainen) -100rpm - 100rpm
* Green Cartridge: (vihreä) -200rpm - 200rpm
* Blue Cartridge: (sininen) -600rpm - 600rpm

<advanced>
</advanced>
