category: sensing  
signature: drivetrain.rotation(DEGREES)
description: Reports the Drivetrain's angle of rotation when configured with a Gyro or Inertial Sensor  

# Drive Rotation
 
Reports the Drivetrain's angle of rotation when configured with a Gyro or Inertial Sensor.

```python
drivetrain.rotation(DEGREES)
```

## How To Use

When configured with a Gyro Sensor, the Drivetrain's `Drive Rotation` command reports an increasingly **positive** value when the Drivetrain turns in the **counter-clockwise** direction.

Conversely, when configured with an Inertial Sensor, `Drive Rotation` reports an increasingly **positive** value when the Drivetrain turns in the **clockwise** direction.
	
<advanced>
</advanced>
