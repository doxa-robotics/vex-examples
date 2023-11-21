category: sensing  
signature: RANGEFINDER.distance(mm)  
device_class: sonar  
description: Reports the distance of the nearest object from the Ultrasonic Range Finder sensor.

# RangeFinder Etäisyys

Antaa Ultrasonic Range Finder sensorin mittaaman etäisyyden lähimpään havaittuun kohteeseen.

```cpp
RangeFinder.distance(units)
```

## Miten käytetään

`RangeFinder.distance()` antaa arvot välillä **30mm - 3000mm**, jos yksikkönä on `mm`, tai **2 inches - 115 inches**, jos yksikkönä on tuumat `inches`.

```cpp
if (RangeFinderC.distance(mm) < 400.0){
    Drivetrain.stop();
}
```
<advanced>
</advanced>