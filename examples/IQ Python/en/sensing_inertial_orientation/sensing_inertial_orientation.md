category: sensing  
signature: inertial.orientation(TYPE, DEGREES)  
device_class: inertial  
description: Gets an orientation angle of the VEX IQ (2nd generation) Brain's Inertial Sensor  

# Inertial Orientation

Gets an orientation angle of the VEX IQ (2nd generation) Brain's Inertial Sensor.

```python
brain_inertial.orientation(TYPE, DEGREES)
```

## How To Use

The orientation reported is determined by the selected axis (x, y, or z). Replace the **TYPE** parameter with one of the following options:

* **OrientationType.PITCH**: represents **pitch**, which reports a value between -90 to +90 degrees.
* **OrientationType.ROLL**: represents **roll**, which reports a value between -180 to +180 degrees)
* **OrientationType.YAW**: represents **yaw**, which reports a value between -180 to +180 degrees)

---

Pitch is the rotation around the side to side axis.

![IQ_Gen2_Basebot_Pitch](IQ_Gen2_Basebot_Pitch.png)

Roll is the rotation around the front to back axis.

![IQ_Gen2_Basebot_Roll](IQ_Gen2_Basebot_Roll.png)

Yaw is rotation around the vertical axis.

![IQ_Gen2_Basebot_Yaw](IQ_Gen2_Basebot_Yaw.png)

<advanced>
</advanced>
