category: sensing  
signature: motor.position(DEGREES)
description:  Reports the distance the V5 Smart Motor or Motor Group has traveled.

# Motor Position

Reports the current rotational position of the selected V5 Smart Motor or the first motor of the specified Motor Group.

```python
motor.position(UNIT)
```

## How To Use

Motor position reports the position of the V5 Smart Motor or the first motor in a Motor Group in integer numbers for degrees, and decimal numbers for turns.

Acceptable values for `UNIT` are: **DEGREES** or **TURNS**.

<advanced>
</advanced>
