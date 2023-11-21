category: drive  
signature: Drivetrain.setStopping(brake);  
device_class: drivetrain  
description: Sets the brake mode of the Drivetrain.  

# Drivetrain Set Stopping

Sets the brake mode of the Drivetrain.

```cpp
Drivetrain.setStopping(brakeType);
```

## How To Use

Here are possible `brakeType` inputs that you can specify: 

* `brake` will cause the Drivetrain to come to an immediate stop, and will not correct for outside forces.
* `coast` lets the Drivetrain spin gradually to a stop.
* `hold` will cause the Drivetrain to come to an immediate stop, and returns it to its stopped position if moved by an outside force, by using the built-in encoder.

## Example

This example will make the Drivetrain move forward for 3 seconds and then hold its position once stopped.

```cpp
Drivetrain.setStopping(hold);
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>