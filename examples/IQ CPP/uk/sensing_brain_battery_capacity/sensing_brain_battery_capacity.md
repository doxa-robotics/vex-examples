category: sensing  
signature: Brain.Battery.capacity(percent)  
description: Reports the capacity of the VEX IQ robot's battery.

# Battery Capacity

Передає значення заряду акумулятора VEX IQ Brain.

```cpp
Brain.Battery.capacity(percent)
```

## Як це працює

`Brain.Battery.capacity` передає числове значення **integer**, яке показує значення заряду батареї VEX IQ Brain у відсотках `percent` і повертає значення в діапазоні **від 0 до 100**.

## Приклад

Цей приклад грає звук тривоги, якщо рівень ємності акумулятора VEX IQ нижче 25%.

```cpp
if (Brain.Battery.capacity(percent) < 25){
  Brain.playSound(alarm);
}
```

<advanced>
</advanced>