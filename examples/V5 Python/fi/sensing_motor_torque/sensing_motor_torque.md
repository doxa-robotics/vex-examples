category: sensing  
signature: motor.torque(UNITS)
description: Reports the amount of torque (rotational force) a V5 Smart Motor is currently using.

# Moottorin vääntö

Raportoi väännön suuruuden (kääntymisvoiman), jota V5 Äly Moottori nyt käyttää.

```python
motor.torque(UNITS)
```

## Miten käytetään

`motor.torque` antaa arvot välillä **0.0 to 18.6** inch-pounds (InLB) jos yksikön **UNITS** parametrina on `TorqueUnits.INLB`.

Vaihtiehtoisesti arvon välillä **0.0 to 2.1** Newton-metriä (Nm) jos yksikön **UNITS** parametrina on `TorqueUnits.NM`.

<advanced>
</advanced>
