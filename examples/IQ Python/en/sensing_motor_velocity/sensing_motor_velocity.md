category: sensing  
signature: motor.velocity(UNITS)
description: Reports the current velocity of an IQ Motor or the first motor of a Motor Group  

# Motor Velocity

Reports the current velocity of an IQ Motor or the first motor of a Motor Group.

```python
motor.velocity(UNITS)
```

## How To Use

Motor velocity reports a range from **-100 to 100** when **PERCENT** is passed as the **UNITS** parameter, or **-127 to 127** if **RPM** is passed.

<advanced>
</advanced>
