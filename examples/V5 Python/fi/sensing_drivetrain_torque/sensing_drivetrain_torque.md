category: sensing  
signature: drivetrain.torque(units)
description: Reports the amount of torque (rotational force) the Drivetrain is currently using.

# Ajopelin vääntö

Antaa ajopelin väännön (kiertovoiman) arvon.

```python
drivetrain.torque(units)
```

## Miten käytetään

`drivetrain.torque` raportoi arvot välillä **0.0 - 18.6** tuuma-paunaa(InLB) jos yksikön **UNITS** parametrina on `TorqueUnits.INLB`.

Vaihtoehtoisesti raportoi arvot välillä **0.0 - 2.1** Newton-metriä (Nm) jos yksikön **UNITS** parametrina on `TorqueUnits.NM`.

<advanced>
</advanced>
