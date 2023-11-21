category: sensing  
signature: inertial.rotation(DEGREES)  
device_class: inertial
description: Reports a VEX IQ (2nd generation) Brain's Inertial Sensor's current angle of rotation in degrees  

# Inertial Rotation

Reports a VEX IQ (2nd generation) Brain's Inertial Sensor's current angle of rotation in degrees.

```python
brain_inertial.rotation(DEGREES)
```

## How To Use

The `Inertial Rotation` command reports an increasingly **positive** value when the Inertial Sensor turns in the **clockwise** direction.

`Inertial Rotation` reports an increasingly **negative** value when the Inertial Sensor turns in the **counter-clockwise** direction.

## Example

The example below turns a Drivetrain until the Inertial Sensor's rotation value is more than 180 degrees before stopping.

```python
drivetrain.turn(RIGHT)
while not brain_inertial.rotation(DEGREES) > 180:
    wait(0.1, SECONDS)
drivetrain.stop()
```

<advanced>
</advanced>
