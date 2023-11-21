category: motion  
signature: motor.spin(FORWARD, 10.0, VOLT)  
device_class: motor  
description: Spins a V5 Smart Motor or Motor Group at a specified voltage.  

# Motor Spin At Voltage
Spins a V5 Smart Motor or Motor Group at a specified voltage.

```python
motor.spin(FORWARD, 10.0, VOLT)
```

## How To Use

**Spin at voltage** accepts a range from -12V to 12V.

Use the `FORWARD` parameter to drive the V5 Smart Motor or Motor Group in the forward direction.

```python
motor.spin(FORWARD, 10.0, VOLT)
```

Use the `REVERSE ` parameter to drive the V5 Smart Motor or Motor Group in the reverse direction.

```cpp
motor.spin(REVERSE, 10.0, VOLT)
```

Spinning a Motor or Motor Group at a negative voltage will cause the Motor/Motor Group to spin in the opposite direction than the one specified.

<advanced>
</advanced>