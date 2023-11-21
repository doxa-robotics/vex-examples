category: drivetrain
signature: drivetrain.set_stopping(MODE)
description: Sets the behavior of the IQ robot's Drivetrain once it stops moving  

# Set Stopping

```python
drivetrain.set_stopping(MODE)
```

## How to Use

Replace the `MODE` parameter with one of the following options:

* BRAKE: will cause the Drivetrain to come to an immediate stop.
* COAST: lets the Drivetrain slow gradually to a stop.
* HOLD: will cause the Drivetrain to come to an immediate stop, and returns it to its stopped position if moved. 

The brake mode applied by the `Set Stopping` command will be applied to subsequent Drivetrain `Stop` commands in the program unless otherwise changed.

## Example

This example shows the robot driving forward for 2 seconds before coasting to a stop.

```python
drivetrain.set_stopping(COAST)
drivetrain.drive(FORWARD)
wait(2, SECONDS)
drivetrain.stop()
```

<advanced>
</advanced>
