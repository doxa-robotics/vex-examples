category: sensing  
signature: LIGHT.brightness()  
device_class: light  
description: Reports the amount of light detected by the Light Sensor.

# Valon kirkkaus

Antaa Light Sensorin havaitseman valon kirkkauden.

```cpp
Light.brightness()
```

## Miten käytetään

`Light.brightness()` antaa arvot välillä **0% - 100%**.

Iso kirkkausarvo vastaa hyvää valaistusarvoa.

Pieni kirkkausarvo vastaa huonoa valaistusarvoa.

Oletusyksikkö on `percent` (5) ja arvot ovat välillä **0% - 100%**.

```cpp
Brain.Screen.print("%d", LightC.brightness());
```
<advanced>
</advanced>