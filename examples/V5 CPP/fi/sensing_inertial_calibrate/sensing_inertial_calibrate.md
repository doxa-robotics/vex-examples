category: sensing  
signature: INERTIAL.calibrate();  
device_class: inertial  
description: Calibrating the Inertial Sensor is used to reduce the amount of drift generated by the Inertial Sensor.

# Inertial kalibrointi

Kalibroimalla Inertial Sensori vähennetään sen mittausarvojen huojuntaa.

```cpp
Inertial.calibrate()
```

Huojuntaa esiintyy, kun Inertial Sensori virheellisesti havaitsee akselien suunnassa arvojen muuitosta vaikka se on levossa.

## How To Use

Inertial Sensorin pitää olla levossa kalibroinnin ajan noin 2 sekuntia.


<advanced>
</advanced>