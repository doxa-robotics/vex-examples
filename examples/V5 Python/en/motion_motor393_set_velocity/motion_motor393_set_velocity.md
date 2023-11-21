category: motion  
signature: motor393.set_velocity(10, PERCENT)  
description: Sets the speed of a Motor393.

# Set Motor Controller Velocity

Sets the speed of a Motor393 connected to a Motor Controller 29.

```python
motor393.set_velocity(VELOCITY, PERCENT)
```

## How To Use

The `VELOCITY` parameter accepts a range of -100% to 100%.

Setting a Motor393's velocity to a negative value will cause the Motor393 to spin in reverse.

The sequence below will cause the Motor393 to spin in reverse, even though the `FORWARD` parameter is passed.

```python
motor393.set_velocity(-100, PERCENT)
motor393.spin(FORWARD)
```

Setting a Motor393's velocity to 0 will prevent the Motor from spinning.

<advanced>
</advanced>
