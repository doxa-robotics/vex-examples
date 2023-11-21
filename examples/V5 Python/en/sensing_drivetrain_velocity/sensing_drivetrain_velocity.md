category: sensing  
signature: drivetrain.velocity(UNITS)
description: Reports the current velocity of the Drivetrain.

# Drive Velocity
 
Reports the current velocity of the Drivetrain.

```python
drivetrain.velocity(UNITS)
```

## How To Use

`drivetrain.velocity` returns a decimal value representing the current velocity of the Drivetrain.

Acceptable `UNITS` are **PERCENT** and **RPM**.

If the provided `UNITS` parameter is **PERCENT**, the reported values ranges between **-100% to 100%**.

Alternatively, if the provided `UNITS` is **RPM**, the range of reported values vary based on the Gear Cartridge installed in the V5 Smart Motors used in the Drivetrain.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

<advanced>
</advanced>
