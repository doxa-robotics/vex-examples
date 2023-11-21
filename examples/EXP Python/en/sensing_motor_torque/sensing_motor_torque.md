category: sensing  
signature: motor.torque(UNITS)
description: Reports the amount of torque (rotational force) a EXP Smart Motor or Motor Group is currently using.

# Motor Torque

Reports the amount of torque (rotational force) a EXP Smart Motor or the first motor of a Motor Group is currently using.

```python
motor.torque(UNITS)
```

## How To Use

`motor.torque` reports a range from **0.0 to 18.6** inch-pounds (InLB) if the provided **UNITS** parameter is `TorqueUnits.INLB`.

Alternatively, a range from **0.0 to 2.1** Newton-meters (Nm) is reported if the provided **UNITS** parameter is `TorqueUnits.NM`.

<advanced>
</advanced>
