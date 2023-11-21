category: sensing  
signature: gyro.rotation(DEGREES)  
device_class: gyro  
description: Reports a VEX IQ Gyro Sensor's current rotation in degrees  

# Gyro Rotation

Reports a VEX IQ Gyro Sensor's current rotation in degrees.

```python
gyro.rotation(DEGREES)
```

## How To Use

`Gyro Rotation` reports an increasing value when the Gyro Sensor turns in the **counter-clockwise** direction.

`Gyro Rotation` reports a decreasing value when the Gyro Sensor turns in the **clockwise** direction.

## Example

The example below prints the rotation of the Gyro Sensor to the VEX IQ brain's screen.

```python
drivetrain.turn(LEFT)

while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("Rotation:", gyro.rotation(DEGREES))

    # Brief delay to prevent print distortion or tearing
    wait(0.1, SECONDS)
```

<advanced>
</advanced>