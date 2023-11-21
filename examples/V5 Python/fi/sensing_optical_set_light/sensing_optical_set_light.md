category: sensing  
signature: optical.set_light(LedStateType.ON)
description: Sets the light on the Optical Sensor to on or off.


# Aseta Optical Valo päälle


Asettaa valon Optical Sensoriin , joko **on** (päälle) tai **off** (pois päältä).

```don
optical.set_light(LedStateType.ON)
```

## Miten käytetään

`optical.set_light(LedStateType.ON)` antaa laittaa Optical Sensorin valon joko **on** (päälle) tai **off** (pois). Näin voit havaita kohteen paremmin, jos yleisvalaistus on huono sensorin edessä.

Parametri **on** on valinta `LedStateType.ON`

```
optical.set_light(LedStateType.ON)
```

Parametri **off** on valinta `LedStateType.OFF`

```
optical.set_light(LedStateType.OFF)
```

<advanced>
</advanced>