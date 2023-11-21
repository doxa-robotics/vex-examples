category: sensing  
signature: GPS.calibrate();  
device_class: gps  
description: Starts the calibration process for a GPS Sensor.  

# GPS Calibrate

Starts the calibration process for a GPS Sensor.

```cpp
GPS.calibrate();
```

## How To Use

The GPS Sensor must remain still during the calibration process.

```cpp
int main() {
  // Calibrate the GPS sensor before starting any program code
  GPS.calibrate();
}
```

<advanced>
</advanced>