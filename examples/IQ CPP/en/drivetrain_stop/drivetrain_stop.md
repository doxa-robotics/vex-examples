category: drive  
signature: Drivetrain.stop();  
device_class: drivetrain  
description: Stops the Drivetrain.  

# Stop

Stops the Drivetrain.

```cpp
Drivetrain.stop();
```

## How To Use

The `Drivetrain.stop` command will cause the Drivetrain to come to a stop.

The stopping behavior can be set with the `Drivetrain.setStopping` command.

## Example

This example will move the VEX IQ robot forward for 3 seconds then come to a stop.

```cpp
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>