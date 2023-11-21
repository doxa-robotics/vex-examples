category: sensing  
signature: DISTANCE.objectVelocity()  
device_class: distance  
description: Reports the velocity of a detected object in m/s  

# Distance Object Velocity

Reports the velocity of a detected object in m/s.

```cpp
Distance.objectVelocity()
```

## How To Use

`Distance.objectVelocity()` reports the current velocity of an object in m/s (meters per second).

The velocity of a detected object will change when the object is moving while in the range of the Distance Sensor.

```cpp
Brain.Screen.print("%.2f", Distance.objectVelocity());
```

<advanced>
</advanced>






