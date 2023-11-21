category: sensing  
signature: motor.velocity(UNITS)
description: Reports the current velocity of a V5 Smart Motor or Motor Group.

# Motor Velocity

Reports the current velocity of a V5 Smart Motor or the first motor of a Motor Group.

```python
motor.velocity(UNITS)
```

## How To Use

Motor velocity reports a range from **-100% to 100%** or **-600rpm to 600rpm**.

Acceptable values for `UNIT` parameter are: **PERCENT** or **RPM**.

Motor velocity will report a "rotations per minute" range based on the Gear Cartridge installed in a V5 Smart Motor or the first motor of a Motor Group.

* Red Cartridge: -100rpm to 100rpm
* Green Cartridge: -200rpm to 200rpm
* Blue Cartridge: -600rpm to 600rpm

<advanced>
</advanced>
