category: sensing  
signature: drivetrain.torque(units)
description: Reports the amount of torque (rotational force) the Drivetrain is currently using.

# Drive Torque

Reports the amount of torque (rotational force) the Drivetrain is currently using.

```python
drivetrain.torque(units)
```

## How To Use

`drivetrain.torque` reports a range from **0.0 to 18.6** inch-pounds (InLB) if the provided **UNITS** parameter is `TorqueUnits.INLB`.

Alternatively, a range from **0.0 to 2.1** Newton-meters (Nm) is reported if the provided **UNITS** parameter is `TorqueUnits.NM`.

<advanced>
</advanced>
