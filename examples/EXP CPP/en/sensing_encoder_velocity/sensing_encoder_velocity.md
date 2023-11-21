category: sensing  
signature: ENCODER.velocity(dps)  
device_class: encoder  
description: Reports the current velocity of a Shaft Encoder.

# Encoder Velocity

Reports the current velocity of a Shaft Encoder.

```cpp
Encoder.velocity(units)
```

## How To Use

`Encoder.velocity()` reports a decimal value (as a *double*) in either degrees per second (`dps`) or rotations per minute (`rpm`).

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Values can be returned in degrees per second (`dps`).

```cpp
Brain.Screen.print("%f", EncoderC.velocity(dps));
```

Values can be returned in rotations per minute (`rpm`).

```cpp
Brain.Screen.print("%f", EncoderC.velocity(rpm));
```
<advanced>
</advanced>