category: sensing  
signature: Brain.Battery.capacity()  
description: Reports the capacity of the EXP Brain's battery.

# Brain Battery Capacity

Reports the current capacity of the EXP robot's battery.

```cpp
Brain.Battery.capacity(percent)
```

## How To Use

`Brain.Battery.capacity` returns an **integer** that represents the EXP robot's battery capacity in the default unit of `percent`, and will return a value in the range of **0 to 100**.

## Example

This example will play an alarm sound if the EXP robot's battery level is lower than 25%.

```cpp
if (Brain.Battery.capacity(percent) < 25){
  Brain.playSound(alarm);
}
```


<advanced>
</advanced>