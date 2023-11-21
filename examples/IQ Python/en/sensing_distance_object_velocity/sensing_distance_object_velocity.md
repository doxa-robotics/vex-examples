category: sensing  
signature: distance.object_velocity()  
device_class: distance  
description: Reports the velocity of a detected object in m/s  

# Distance Object Velocity

Reports the velocity of a detected object in m/s.

```python
distance.object_velocity()
```

## How To Use

`Distance Object Velocity` reports the current velocity of an object in m/s (meters per second).

The velocity of a detected object will change when the object is moving while in the range of an IQ Distance Sensor (2nd generation).

```python
brain.screen.print("Velocity:", distance.object_velocity())
```

<advanced>
</advanced>






