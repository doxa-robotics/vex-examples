category: sensing  
signature: Drivetrain.rotation()  
device_class: smartdrive  
description: Reports the Drivetrain's angle of rotation when configured with a 3-Wire Gyro Sensor or V5 Inertial Sensor.

# Ajopelin käännöskulma

Antaa ajopelin käännöskulman joko 3-lankagurolla tai V5 Inertial Sensorilla mitattuna.

```cpp
Drivetrain.rotation()
```

## Miten käytetään

`Drivetrain.rotation()` antaa **positiivisen** arvon, jos ajopeli kääntyy **myötäpäivään**.

`Drivetrain.rotation()` antaa **nagatiivisen** arvon, jos ajopeli kääntyy **vastapäivään**.

```cpp
waitUntil(Drivetrain.rotation() > 180);
```
<advanced>
</advanced>
