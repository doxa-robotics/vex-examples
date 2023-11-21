category: sensing  
signature: Motor.current(units)  
device_class: motor  
description: Reports the amount of current a Motor is currently using.

# Motor Current

Передає кількість струму, яку мотор VEX IQ зараз використовує.

```cpp
Motor.current(units)
```

## Як це працює

`Motor.current` передає десяткове значення (*double*) кількості струму, яку зараз використовує мотор.

Команда `Motor.current` приймає параметр одиниць вимірювання `units` **amp** (ампери) або **percent**.

Друкування струму мотору у відсотках:

```cpp
Brain.Screen.print("%f" , Motor.current(percent));
```

Друкування струму мотору в амперах:

```cpp
Brain.Screen.print("%f", Motor.current(amp));
```

<advanced>
</advanced>