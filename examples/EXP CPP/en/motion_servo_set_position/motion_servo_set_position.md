category: motion  
signature: SERVO.setPosition(90, degrees);  
device_class: servo
description: Spins a EXP Servo Motor to a set position.  

# Servo Set Position

Spins a EXP Servo Motor to a set position.

```cpp
Servo.setPosition(position, degrees);
```

## How To Use

Spins a servo motor to the given positional value.

The `Servo.setPosition()` command accepts a range of values from **-50** to **50** for the **position** parameter.


## Example

This example spins the servo motor to 25 degrees, waits 2 seconds, then spins the motor to -25 degrees.

```cpp
Servo.setPosition(25, degrees);
wait(2, seconds);
Servo.setPosition(-25, degrees);
```

<advanced>
</advanced>