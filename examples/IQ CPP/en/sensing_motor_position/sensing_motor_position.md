category: sensing  
signature: Motor.position(units)  
device_class: motor  
description: Reports the current position of the Motor or Motor Group.

# Motor Position

Reports the current position of the encoder in the specified VEX IQ Smart Motor or the first motor in a Motor Group.

```cpp
Motor.position(units)
```

## How To Use

`Motor.position` returns a decimal value (as a *double*) to report the position of the encoder in a Motor or in the first motor of a Motor Group.

Replace the `units` parameter with either **degrees** or **turns**.

Values can be returned in **degrees**.

```cpp
Brain.Screen.print("Motor Position (Degrees): %.2f", Motor.position(degrees));
```

Values can be returned in **turns**.

```cpp
Brain.Screen.print("Motor Position (Turns): %.2f", Motor.position(turns));
```

<advanced>
</advanced> 