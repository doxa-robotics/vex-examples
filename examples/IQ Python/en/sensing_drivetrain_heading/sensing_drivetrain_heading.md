category: sensing  
signature: drivetrain.heading(DEGREES)
description: Reports the direction that the Drivetrain is facing by using the Gyro or Inertial Sensor's current angular position  

# Drive Heading
 
Reports the direction that the Drivetrain is facing by using the Gyro or Inertial Sensor's current angular position.

```python
drivetrain.heading(DEGREES)
```

## How To Use

Drive heading reports a range from **0.00 to 359.99 degrees**.

When the Drivetrain is configured with a Gyro Sensor, the `Drive Heading` command reports an increase in heading when rotating counter-clockwise.

Alternatively, if the Drivetrain is configured with the IQ (2nd generation) Brain's Inertial Sensor, the `Drive Heading` command reports an increase in heading when rotating clockwise.
	
<advanced>
</advanced>
