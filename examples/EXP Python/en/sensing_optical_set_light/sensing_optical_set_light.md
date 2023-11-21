category: sensing  
signature: optical.set_light(LedStateType.ON)
description: Sets the light on the Optical Sensor to on or off.


# Set Optical Light
Sets the light on the Optical Sensor to **on** or **off**.

```don
optical.set_light(LedStateType.ON)
```

## How To Use
`optical.set_light(LedStateType.ON)` allows you to turn the Optical Sensor's light **on** or **off**. The light lets the sensor see objects if it is looking at an object in a dark area.

To turn the light **on** you pass `LedStateType.ON`

```
optical.set_light(LedStateType.ON)
```

To turn the light **off** you pass `LedStateType.OFF`

```
optical.set_light(LedStateType.OFF)
```

<advanced>
</advanced>