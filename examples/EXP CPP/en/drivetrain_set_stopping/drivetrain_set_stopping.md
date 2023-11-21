category: drive  
signature: Drivetrain.setStopping(brake);  
device_class: drivetrain  
description: Sets the brake mode of the Drivetrain.  

# Drivetrain Set Stopping

Here are the valid inputs for the `brakeType` parameter that you can specify: 

* **brake** will cause the Drivetrain to come to an immediate stop, and will not correct for outside forces.
* **coast** lets the Drivetrain slow gradually to a stop.
* **hold** will cause the Drivetrain to come to an immediate stop, and returns it to its stopped position if moved by an outside force.

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