category: drive  
signature: Drivetrain.driveFor(forward, 1, inches);  
device_class: drivetrain  
description: Moves the Drivetrain for a given distance.  

# Drive For

Moves the Drivetrain for a given distance. 

```cpp
Drivetrain.driveFor(direction, distance, units);
```

## How To Use

Choose which `direction` the Drivetrain will move - either **forward** or **reverse**. 

Set how far the Drivetrain will move by entering a numeric value for `distance`. 

Then, specify the `units` of measurement as either **inches** or **mm**.

```cpp
Drivetrain.driveFor(reverse, 5, inches);
```

The `Drivetrain.driveFor` command will by default block other commands until the Drivetrain movement has completed.

## Optional Parameters

You can set `false` as the last parameter to prevent the `Drivetrain.driveFor` command from blocking the program until the movement has completed.

```cpp
Drivetrain.driveFor(forward, 200, mm, false);
```

<advanced>
</advanced>
