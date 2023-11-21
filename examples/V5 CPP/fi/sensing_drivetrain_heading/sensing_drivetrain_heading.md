category: sensing  
signature: Drivetrain.heading()  
device_class: smartdrive  
description: Reports the 3-Wire Gyro Sensor or V5 Inertial Sensor's current heading in degrees.

# Ajopelin ajosuunta

Antaa 3-lanka Gyro Sensorilla tai V5 Inertial Sensorilla nykyisen ajosuunnan asteina.

```cpp
Drivetrain.heading()
```

## Miten käytetään

`Drivetrain.heading()` antaa kasvavia arvoja ajosuunnssa kun ajopeli kääntyy myötäpäivään.

`Drivetrain.heading()` antaa arvot välillä **0.00 - 359.99**.

```cpp
waitUntil(Drivetrain.heading() > 180);
```
<advanced>
</advanced>
