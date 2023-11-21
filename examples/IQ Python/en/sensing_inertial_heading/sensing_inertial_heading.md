category: sensing  
signature: inertial.heading(DEGREES)  
device_class: inertial  
description: Reports a VEX IQ (2nd generation) Brain's Inertial Sensor's current heading in degrees  

# Inertial Heading

Reports a VEX IQ (2nd generation) Brain's Inertial Sensor's current heading in degrees.

```python
brain_inertial.heading(DEGREES)
```

## How To Use

The `Inertial Heading` command reports an increase in heading when rotating clockwise.

`Inertial Heading` reports a range of values from **0.00 to 359.99** degrees.

## Example

The example below turns a Drivetrain until the Inertial Sensor's heading value is more than 180 degrees before stopping.

```python
drivetrain.turn(RIGHT)
while not brain_inertial.heading(DEGREES) > 180:
    wait(0.1, SECONDS)
drivetrain.stop()
```

<advanced>
</advanced>
