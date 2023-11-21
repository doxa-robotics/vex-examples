category: sensing  
signature: OPTICAL.setLightPower(100, percent);  
device_class: optical  
description: Sets the intensity of a V5 Optical Sensor's LED  

# Optical Set Light Power

Sets the intensity of a V5 Optical Sensor's LED.

```cpp
Optical.setLightPower(power, percent);
```

## How To Use

`Optical.setLightPower()` can be used to set the intensity of the LED on the V5 Optical Sensor.

It accepts a range of values from **0 to 100** as the first parameter.

The second parameter is **percent**.

A higher value will increase the intensity of the LED, while a lower value will decrease the intensity.

```cpp
Optical.setLightPower(100, percent);
Optical.setLight(ledState::on);
```

<advanced>
</advanced>







