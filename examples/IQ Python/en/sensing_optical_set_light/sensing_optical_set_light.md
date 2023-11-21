category: sensing  
signature: optical.set_light(STATE)  
device-class: optical  
description: Sets the light on a VEX IQ Optical Sensor to on or off  

# Set Optical Light

Sets the light on a VEX IQ Optical Sensor to **on** or **off**.

```python
optical.set_light(STATE)
```

## How To Use

`Set Optical Light` allows you to turn the Optical Sensor's light **on** or **off**. The light lets the sensor see objects if it is looking at an object in a dark area.

To turn the light **on** you pass `LedStateType.ON` as the **STATE** parameter.

```
optical.set_light(LedStateType.ON)
```

To turn the light **off** you pass `LedStateType.OFF` as the **STATE** parameter.

```
optical.set_light(LedStateType.OFF)
```

<advanced>
</advanced>