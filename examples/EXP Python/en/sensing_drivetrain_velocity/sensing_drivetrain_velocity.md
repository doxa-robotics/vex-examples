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

Alternatively, if the provided `UNITS` is **RPM**, the range of reported values vary based on Smart Motors used in the Drivetrain.

<advanced>
</advanced>
