category: sensing  
signature: LINETRACKER.reflectivity()  
device_class: line  
description: Reports the amount of light reflected using the Line Tracker sensor.

# Viivanseuraaja valonheijastus

Antaa valon määrän jonka viivanseuraaja havaitsee.

```cpp
LineTracker.reflectivity()
```

## Miten käytetän

Vaaleat valopinnat heijastavat valoa enenmmän kun tummat ja antavat isompia arvoja.

Oletusyksikkö on `percent` ja valonheijastusarvot vaihtelevat välillä **0% - 100%**.

```cpp
Brain.Screen.print("%d", LineTrackerA.reflectivity());
```
<advanced>
</advanced>