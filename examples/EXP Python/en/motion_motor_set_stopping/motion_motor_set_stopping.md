category: motion  
signature: motor.set_stopping(BRAKE)  
description: Sets the behavior of the EXP Smart Motor or Motor Group once it stops moving.

# Set Motor Stopping

Sets the stopping behavior of a EXP Smart Motor or Motor Group.

```python
motor.set_stopping(MODE)
```

## How To Use

The `MODE` parameter can be replaced with any of the following options:

* BRAKE: will cause the Motor/Motor Group to come to an immediate stop.
* COAST: lets the Motor/Motor Group spin gradually to a stop.
* HOLD: will cause the Motor/Motor Group to come to an immediate stop, and returns it to its stopped position if moved.

The stopping behavior set by this command will apply to subsequent motion commands for the entirety of the project, unless otherwise changed.

## Example

This example will make the Arm Motor spin forward for 90 degrees (to raise the arm) and then will hold its position.

```python
arm_motor.set_stopping(HOLD)
arm_motor.spin_for(FORWARD, 90, DEGREES)
```

<advanced>
</advanced>
