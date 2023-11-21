category: drivetrain
signature: drivetrain.set_stopping(BRAKE)
description: Sets the behavior of the EXP robot's Drivetrain once it stops moving.  

# Set Stopping

```python
drivetrain.set_stopping(MODE)
```

## How to Use

Replace the `MODE` parameter with one of the following options:

* BRAKE: will cause the Drivetrain to come to an immediate stop.
* COAST: lets the Drivetrain slow gradually to a stop.
* HOLD: will cause the Drivetrain to come to an immediate stop, and returns it to its stopped position if moved. 

The brake mode applied by the `drivetrain.set_stopping()` command will be used for subsequent Drivetrain commands in the program unless otherwise changed.

## Example

This example shows the robot driving forward for 200 MM before coasting to a stop.

```python
drivetrain.set_stopping(COAST)
drivetrain.drive_for(FORWARD, 200, MM)
```
<advanced>
</advanced>
