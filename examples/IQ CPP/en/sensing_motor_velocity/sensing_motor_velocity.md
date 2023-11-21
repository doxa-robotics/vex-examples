category: sensing  
signature: Motor.velocity(units)  
device_class: motor  
description: Reports the current velocity of the Motor or Motor Group.  

# Motor Velocity

Reports the velocity of the specified VEX IQ Smart Motor or of the first motor in a Motor Group.

```cpp
Motor.velocity(units)
```

## How to Use

`Motor.velocity` returns a decimal value (as a *double*) to report the current velocity of a Motor or of the first motor in a Motor Group. 

Specify the `units` when using this command.

**percent** - will return a value from **-100% to 100%**.
 
```cpp
Brain.Screen.print("%f", Motor.velocity(percent));
```
  
`Motor.velocity` can also return values in **rpm** (revolutions per minute).

```cpp
Brain.Screen.print("%f", Motor.velocity(rpm));
``` 

<advanced>
</advanced>