category: sensing  
signature: Drivetrain.velocity(units)  
device_class: drivetrain
description: Reports the current velocity of the Drivetrain.

# Drivetrain Velocity

Reports the current velocity of the Drivetrain.

```cpp
Drivetrain.velocity(units)
```

## How to Use
`Drivetrain.velocity` returns a decimal value (as a *double*) to report the current velocity of the Drivetrain. 

`Drivetrain.velocity` returns a value from **-100% to 100%** if the provided `units` is **percent**.

`Drivetrain.velocity` can also take **rpm** (revolutions per minute) as the provided `units` parameter.

If a negative value is returned, it means that the Drivetrain is currently moving in reverse.

## Example

The example below prints the Drivetrain's velocity (in percent) to the VEX IQ's Brain.

```cpp
Brain.Screen.print("%f", Drivetrain.velocity(percent));
```

<advanced>
</advanced>