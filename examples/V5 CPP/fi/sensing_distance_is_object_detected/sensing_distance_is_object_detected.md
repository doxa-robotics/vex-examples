category: sensing  
signature: DISTANCE.isObjectDetected()  
device_class: distance  
description: Reports if a V5 Distance Sensor detects an object or surface in its range  

# Havaittu esine

Antaa tiedon jos V5 Etäisyysanturi havaitsee esineen näkökentässään.

```cpp
Distance.isObjectDetected()
```

## Miten käytetään

`Distance.isObjectDetected()` antaa arvon **TRUE** jos esine tai heijastava pinta onnäkökentässä ja muuten arvon **false**.

Alla tulostetaan **TRUE** or **FALSE** riippuen onko esine havaittu.

```cpp
Brain.Screen.print("%s", Distance.isObjectDetected() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>




