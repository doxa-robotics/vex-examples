category: drive  
signature: Drivetrain.turnFor(right, 90, degrees);  
device_class: drivetrain  
description: Turns the Drivetrain for a distance.  

# Drivetrain Turn For

Turns the Drivetrain for the specified angle and direction.

```cpp
Drivetrain.turnFor(direction, angle, degrees);
```

## How To Use

Set the `direction` and amount the Drivetrain will turn by entering a direction - **left** or **right**, and a number of degrees.

```cpp
Drivetrain.turnFor(right, 270, degrees);
```

The `Drivetrain.turnFor` command will by default block other commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `false` as the last parameter to prevent the `Drivetrain.turnFor` command from blocking the program until the movement has completed.

```cpp
Drivetrain.turnFor(left, 90, degrees, false);
```

<advanced>
</advanced>
