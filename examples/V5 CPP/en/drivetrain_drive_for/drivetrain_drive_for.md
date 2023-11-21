category: drive  
signature: Drivetrain.driveFor(forward, 200, mm);  
device_class: drivetrain  
description: Moves the Drivetrain for a given distance.  

# Drivetrain Drive For

Moves the Drivetrain for a given distance. All drivetrain motors are run forwards or backwards at the speed that was set using `Drivetrain.setDriveVelocity`. After the drivetrain has moved the requested distance the motors are stopped.

```cpp
Drivetrain.driveFor(directionType, distance, distanceUnits);
```

## How To Use

Set how far the Drivetrain will move by entering a direction (`forward` or `reverse`) with a value and specifying the unit of measurement (`inches` or `mm`).

The `Drivetrain.driveFor();` accepts numeric values for `distance`.

```cpp
Drivetrain.driveFor(reverse, 5.0, inches);
```

The **driveFor** command will block other commands until the Drivetrain movement has completed.

## Optional Parameters

You can set `false` as the last parameter to tell the **driveFor** command to not block the program until the movement has completed.

```cpp
Drivetrain.driveFor(forward, 5.0, inches, false);
```

<advanced>
</advanced>
