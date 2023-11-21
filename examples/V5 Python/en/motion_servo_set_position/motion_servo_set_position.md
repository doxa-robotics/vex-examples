category: motion  
signature: servo.set_position(50, DEGREES)  
description: Sets the Servo's encoder position to the given value.

# Spin Servo

Spins a Servo Motor to a set position.

```python
servo.set_position(POSITION, DEGREES)
```

## How To Use

The `servo.set_position()` command accepts a range of values from **-50** to **50** for the **POSITION** parameter.

## Example

The below example spins the servo motor to 25 degrees, waits 2 seconds, then spins the motor to -25 degrees.

```python
servo.set_position(25, DEGREES)
wait(2, SECONDS)
servo.set_position(-25, DEGREES)
```

<advanced>
</advanced>
