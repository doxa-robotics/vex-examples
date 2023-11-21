category: drive  
signature: Drivetrain.turnFor(right, 90, degrees);  
device_class: drivetrain  
description: Turns the Drivetrain for a distance.  

# Drivetrain Turn For

`Drivetrain.turnFor()` causes the Drivetrain to turn for the requested angle and direction.

```cpp
Drivetrain.turnFor(turnType, angle, units);
```

## How To Use

Set how far the Drivetrain will move by entering a direction (`left` or `right`) and a number of degrees.

```cpp
Drivetrain.turnFor(right, 270, degrees);
```

The **turnFor** command will block other commands until the Drivetrain turn has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the **turnFor** command to not block the program until the movement has completed.

```cpp
Drivetrain.turnFor(left, 90, degrees, false);
```

<advanced>
</advanced>
