category: sensing  
signature: GPS.orientation(roll, degrees)  
device_class: gps  
description: Reports the angle of the specified orientation axis on a GPS Sensor.  

# GPS Orientation

Reports the angle of the specified orientation axis on a GPS Sensor.

```cpp
GPS.orientation(axis, degrees)
```

## How To Use

`GPS.orientation()` reports a *double* representing the angle of rotation about the specified orientation `axis`:

* The **roll** axis reports a value between **-180** to **+180** degrees, representing the angle of a GPS Sensor when tilted left or right

* The **pitch** axis reports a value between **-90** to **+90** degrees, representing the angle of a GPS Sensor when tilted forward or backwards

* The **yaw** axis reports a value between **-180** to **+180** degrees, representing the angle of a GPS Sensor when rotated about the vertical axis

## Example

```cpp
// Print the yaw orientation in a loop
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("GPS Yaw Orientation: %f", GPS.orientation(yaw, degrees));
  wait(0.1, seconds);
}
```

<advanced>
</advanced>