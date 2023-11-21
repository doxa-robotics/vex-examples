category: sensing  
signature: GPS.acceleration(xaxis)  
device_class: gps  
description: Reports the acceleration value of the specified axis on a GPS Sensor.  

# GPS Acceleration

Reports the acceleration value of the specified axis on a GPS Sensor.

```cpp
GPS.acceleration(axis)
```

## How To Use

The `GPS.acceleration()` command reports a decimal value (as a *double*) in the range of **-4.0** to **4.0** Gs.

It can report acceleration values from three different axes based on the value passed as the `axis` parameter:

* The **xaxis** reports the acceleration value of a GPS Sensor's forward and backward rotations

* The **yaxis** reports the acceleration value of a GPS Sensor's left and right rotations

* The **zaxis** reports the acceleration value of a GPS Sensor's up and down movements

```cpp
Brain.Screen.print("Acceleration on X: %f", GPS.acceleration(xaxis));
```

<advanced>
</advanced>