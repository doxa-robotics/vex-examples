category: sensing  
signature: Brain.Battery.capacity(percent)  
description: Reports the capacity of the VEX IQ robot's battery.

# Battery Capacity

Reports the current capacity of the VEX IQ robot's battery.

```cpp
Brain.Battery.capacity(percent)
```

## How To Use

`Brain.Battery.capacity` returns an **integer** that represents the VEX IQ robot's battery capacity in the default unit of `percent`, and will return a value in the range of **0 to 100**.

## Example

This example will play an alarm sound if the VEX IQ robot's battery level is lower than 25%.

```cpp
if (Brain.Battery.capacity(percent) < 25){
  Brain.playSound(alarm);
}
```

<advanced>
</advanced>