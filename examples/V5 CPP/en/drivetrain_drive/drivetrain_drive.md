category: drive  
signature: Drivetrain.drive(forward);  
device_class: drivetrain  
description: Moves the Drivetrain forever. All drivetrain motors are run forwards or backwards at the speed that was set using `Drivetrain.setDriveVelocity`, the default speed is 50 rpm.

# Drivetrain Drive

Moves the Drivetrain forever. All drivetrain motors are run forwards or backwards at the speed that was set using `Drivetrain.setDriveVelocity`, the default speed is 50 rpm.

```cpp
Drivetrain.drive(directionType);
```

## How To Use

The `Drivetrain.drive();` command will run the Drivetrain forever, until a new Drivetrain command is used, or the program is stopped.

Use the `forward` parameter to drive the Drivetrain in the forward direction.

```cpp
Drivetrain.drive(forward);
```

Use the `reverse` parameter to drive the Drivetrain in the reverse direction.

```cpp
Drivetrain.drive(reverse);
```
 
<advanced>
</advanced>