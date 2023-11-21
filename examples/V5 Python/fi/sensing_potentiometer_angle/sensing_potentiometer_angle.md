category: sensing  
signature: potentiometer.angle(UNITS)
description: Returns the angular position of the Potentiometer.

# Potentiometrin kulma

Palauttaa Potentiometrin mittaaman kulma-asennon.

```don
potentiometer.angle(UNITS)
```

##Miten käytetään

`potentiometer.angle` palauttaa Potentiometrin mittaaman kulman desimaalilukuna.

`UNITS` -yksikköparametri hyväksyy argumentin joko **DEGREES** (asteina) tai **PERCENT** (prosentteina).

'UNITS` yksikkönä **DEGREES** antaa arvoväliltä **0.0 - 250.0 degrees**.

Vastaavasti `UNITS` yksikkönä **PERCENT** palauttaa arvot väliltä **0 - 100%** .

<advanced>
</advanced>
