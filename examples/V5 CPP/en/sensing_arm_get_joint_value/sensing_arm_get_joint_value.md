category: arm  
signature: RoboticArm.getJointValue(1);  
device_class: RoboticArm  
description: Reports the potentiometer value of one of the four joints on the V5 Workcell. 

# Joint potentiometer value

Reports the potentiometer value of one of the four joints on the V5 Workcell.

```cpp
RoboticArm.getJointValue(1);
```

## How To Use

The `RoboticArm.getJointValue(1);` command is used to report the potentiometer value of one of the four joints on the Workcell. This command can be used when determining mastering values.

The `RoboticArm.getJointValue(1);` command reports a range of **0 to 4095**.

Choose which joint to report. There are four joints on the Workcell: 

* **Joint 1:** RoboticArm.getJointValue(1);
* **Joint 2:** RoboticArm.getJointValue(2);
* **Joint 3:** RoboticArm.getJointValue(3);
* **Joint 4:** RoboticArm.getJointValue(4);

<advanced>
</advanced>
