category: sensing  
signature: INERTIAL.calibrate();  
device_class: inertial  
description: Calibrating the Inertial Sensor is used to reduce the amount of drift generated by the Inertial Sensor.

# Inertial Calibrate

Calibrating the Inertial Sensor is used to reduce the amount of drift generated by the Inertial Sensor.

```cpp
Inertial.calibrate();
```

Drifting occurs when the Inertial Sensor incorrectly detects movement even though the sensor is not physically moving.

## How To Use

The Inertial Sensor must remain still during the calibration process. The calibration process will take approximately 2 seconds to complete.


<advanced>
</advanced>
