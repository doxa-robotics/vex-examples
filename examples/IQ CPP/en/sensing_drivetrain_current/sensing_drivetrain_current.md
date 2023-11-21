category: sensing  
signature: Drivetrain.current(units)  
device_class: drivetrain  
description: Reports the amount of current (power) that the Drivetrain is currently using.

# Drivetrain Current

Reports the amount of current that the Drivetrain is currently using.

```cpp
Drivetrain.current(units)
```

## How To Use

`Drivetrain.current` returns a decimal value (as a *double*) to report the amount of current the Drivetrain is currently using.

The `Drivetrain.current` command accepts **amp** (Amperes) as a valid `units` parameter.

## Example

The example below prints the current (in Amperes) of the VEX IQ robot's Drivetrain to the Brain.

```cpp
Brain.Screen.print("%f", Drivetrain.current(amp));
```

<advanced>
</advanced>