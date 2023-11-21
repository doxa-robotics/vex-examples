category: drive  
signature: Drivetrain.stop();  
device_class: drivetrain  
description: Stops the Drivetrain.  

# Drivetrain Stop

Stops the Drivetrain.

```cpp
Drivetrain.stop();
```

## How To Use

The `Drivetrain.stop();` command will cause the Drivetrain to come to a complete stop and use the `Drivetrain.setStopping();` to set either `coast`, `brake`, or `hold` its position.

## Example

This example will stop the Drivetrain after 3 seconds.

```cpp
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>