category: sensing  
signature: POTENTIOMETER.angle(units)  
device_class: pot  
description: Returns the angular position of the Potentiometer.

# Potentiometer Angle

Returns the angular position of the Potentiometer.

```cpp
Potentiometer.angle(units)
```

## How To Use

`Potentiometer.angle()` returns a decimal value (as a *double*) to report the angular position of the Potentiometer.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Set **degrees** as the `units` parameter to get values ranging from **0.0 to 250.0 degrees** for a V5 Potentiometer, or from **0.0 to 330.0 degrees** for a V5 Potentiometer V2.

If the provided `units` parameter is in **percent**, the return values ranges from **0 to 100%**.

```cpp
Brain.Screen.print("%f", PotentiometerA.angle(degrees));
```

<advanced>
</advanced>