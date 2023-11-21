category: sensing  
signature: ENCODER.position(degrees)  
device_class: encoder  
description: Reports the distance the Shaft Encoder has rotated.

# Encoder Position

Reports the distance the Shaft Encoder has rotated.

```cpp
Encoder.position(units)
```

## How To Use

`Encoder.position()` returns a decimal value (as a *double*) to report the distance the Shaft Encoder has rotated.


Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.


Values can be returned in `degrees`.

```cpp
Brain.Screen.print("%f", EncoderC.position(degrees));
```

Values can be returned in `turns`.

```cpp
Brain.Screen.print("%f", EncoderC.position(turns));
```
<advanced>
</advanced>