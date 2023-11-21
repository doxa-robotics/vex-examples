category: sensing  
signature: LINETRACKER.reflectivity()  
device_class: line  
description: Reports the amount of light reflected using the Line Tracker sensor.

# LineTracker Reflectivity

Reports the amount of light reflected using the Line Tracker sensor.

```cpp
LineTracker.reflectivity()
```

## How To Use

Light colored surfaces will reflect more light and will report a high reflectivity value.

Dark colored surfaces will reflect less light and will report a low reflectivity value.

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

The default unit is `percent` that returns an integer value from **0% to 100%**.

```cpp
Brain.Screen.print("%d", LineTrackerA.reflectivity());
```
<advanced>
</advanced>