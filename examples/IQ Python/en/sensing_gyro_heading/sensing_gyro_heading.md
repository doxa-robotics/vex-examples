category: sensing  
signature: gyro.heading(DEGREES)  
device_class: gyro  
description: Reports a VEX IQ Gyro Sensor's current heading in degrees  

# Gyro Heading

Reports a VEX IQ Gyro Sensor's current heading in degrees.

```python
gyro.heading(DEGREES)
```

## How To Use

`Gyro Heading` reports a range of values from **0.00 to 359.99**.

The `Gyro Heading` command reports an increase in heading when rotating **counter-clockwise**.

The `Gyro Heading` command reports a decrease in heading when rotating **clockwise**.

## Example

The example below prints the heading of the Gyro Sensor to the VEX IQ brain's screen.

```python
drivetrain.turn(LEFT)

while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("Heading:", gyro.heading(DEGREES))

    # Brief delay to prevent print distortion or tearing
    wait(0.1, SECONDS)
```

<advanced>
</advanced>