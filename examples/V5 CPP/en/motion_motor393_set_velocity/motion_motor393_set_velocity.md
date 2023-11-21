category: motion  
signature: MOTOR393.setVelocity(50, percent);  
device_class: motor29
description: Sets the speed of a Motor393 connected to a Motor Controller 29. 

# Motor393 Set Velocity

Sets the speed of a Motor393 connected to a Motor Controller 29.

```cpp
Motor393.setVelocity(velocity, percent);
```

## How To Use

The velocity parameter accepts a range of **-100% to 100%.** 

Setting a Motor393's velocity to a negative value will cause the Motor393 to spin in reverse.

The sequence below will cause the Motor393 to spin in reverse, even though the `forward` parameter is passed.

```cpp
Motor393.setVelocity(-100, percent);
Motor393.spin(forward);
```

Setting a Motor393's velocity to 0 will prevent the Motor from spinning.

<advanced>
</advanced>