category: sensing  
signature: OPTICAL.setLight(ledState::on);  
device_class: optical  
description: Sets the state of the Optical Sensor's LED    

# Optical Set Light

Sets the state of the Optical Sensor's LED.

```cpp
Optical.setLight(ledState);
```

## How To Use

`Optical.setLight()` can be used to set the state of the LED on the Optical Sensor.

It accepts either **ledState::on** or **ledState::off** as a parameter.

**ledState::on** will turn the LED on.

**ledState::off** will turn the LED off.

```cpp
Optical.setLight(ledState::on);
wait(2, seconds);
Optical.setLight(ledState::off);
```

<advanced>
</advanced>







