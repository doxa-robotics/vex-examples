category: sensing  
signature: Motor.velocity(units)  
device_class: motor  
description: Reports the current velocity of the motor.  

# Motor Velocity

Повертає поточну швидкість обраного мотора VEX IQ.

```cpp
Motor.velocity(units)
```

## Як це працює

`Motor.velocity` передає десяткове значення (*double*), яке показує поточну швидкість мотора. 

Задайте одиниці вимірювання `units`, коли використовуєте цю команду.

**percent** - повертає значення в діапазоні **від -100% до 100%**.
 
```cpp
Brain.Screen.print("%f", Motor.velocity(percent));
```
  
`Motor.velocity` також повертає значення в діапазоні **від -127 до 127**, коли використано одиниці **rpm** (оберти за хвилину).

```cpp
Brain.Screen.print("%f", Motor.velocity(rpm));
``` 

<advanced>
</advanced>