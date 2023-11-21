category: motion  
signature: Motor.spin(forward, 10.0, volt);  
device_class: motor  
description: Spins a V5 Smart Motor or Motor Group at a specified voltage.  

# Motor Spin At Voltage
Spins a V5 Smart Motor or Motor Group at a specified voltage.

```cpp
Motor.spin(directionType, voltage, volt);
```

## How To Use

**Spin at voltage** accepts a range from -12V to 12V.

Use the `forward` parameter to drive the V5 Smart Motor or Motor Group in the forward direction.

```cpp
Motor.spin(forward, 10.0, volt);
```

Use the `reverse` parameter to drive the V5 Smart Motor or Motor Group in the reverse direction.

```cpp
Motor.spin(reverse, 10.0, volt);
```

Spinning a Motor or Motor Group at a negative voltage will cause the Motor/Motor Group to spin in the opposite direction than the one specified.

<advanced>
</advanced>