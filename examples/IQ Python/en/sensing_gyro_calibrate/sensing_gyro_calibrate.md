category: sensing  
signature: gyro.calibrate(TYPE)   
device_class: gyro  
description: Calibrates a Gyro Sensor to reduce the amount of drift generated by the Gyro Sensor  

# Gyro Calibrate

Calibrates a VEX IQ Gyro Sensor to reduce the amount of drift generated by the Gyro Sensor.

```python
gyro.calibrate(TYPE)
```

Drifting occurs when the Gyro Sensor incorrectly detects movement even though the sensor is not moving.

## How To Use

The Gyro Sensor must remain still during the calibration process.

The **TYPE** parameter can be replaced with any of the following options to set the calibration duration of the Gyro Sensor:

- **GyroCalibrationType.NORMAL** will calibrate the Gyro Sensor for 2 seconds
- **GyroCalibrationType.SLOW** will calibrate the Gyro Sensor for 4 seconds
- **GyroCalibrationType.EXTENDED** will calibrate the Gyro Sensor for 8 seconds

<advanced>
</advanced>