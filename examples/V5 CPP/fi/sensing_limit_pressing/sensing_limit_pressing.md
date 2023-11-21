category: sensing  
signature: LimitSwitch.pressing()  
device_class: limit  
description: Reports if the Limit Switch is pressed.

# LimitSwitch Painettu

Kertoo onko Limit Switch sensoria painettu.

```cpp
LimitSwitch.pressing()
```

## Miten käytetään

`LimitSwitch.pressing()` antaa arvon **true** jos sitä on painettu.

`LimitSwitch.pressing()` antaa arvon **false** jos sitä ei ole painettu.

```cpp
waitUntil(LimitSwitchB.pressing());
``` 
<advanced>
</advanced>
