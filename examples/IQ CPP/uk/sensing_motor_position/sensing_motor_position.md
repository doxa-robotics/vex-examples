category: sensing  
signature: Motor.position(units)  
device_class: motor  
description: Reports the current position of the Motor

# Motor Position

Передає поточну позицію енкодера обраного мотора VEX IQ.

```cpp
Motor.position(units)
```

## Як це працює

`Motor.position` передає десяткове значення (*double*), яке показує позицію енкодера мотора.

Введіть параметр одиниць вимірювання `units` - **degrees** або **turns**.

Отримання значення у відсотках (**degrees**).

```cpp
Brain.Screen.print("Motor Position (Degrees): %.2f", Motor.position(degrees));
```

Отримання значення в обертах (**turns**).

```cpp
Brain.Screen.print("Motor Position (Turns): %.2f", Motor.position(turns));
```

<advanced>
</advanced> 