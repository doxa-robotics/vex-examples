category: looks  
signature: Color.setLight(50, percent);  
device_class: Color Sensor  
description: Sets the brightness of the VEX IQ Color Sensor's light.  

# Set Color Sensor Light

Встановлює яскравість випромінюваного світла датчика кольору VEX IQ.

```cpp
Color.setLight(brightness, percent);
```

## Як це працює

Датчик кольору має джерело світла, яке можна відрегулювати, щоб покращити розпізнавання кольору об'єкта або яскравості поверхні.

`Color.setLight` приймає значення в діапазоні **від 0 до 100** для параметра яскравості `brightness`.

Чим більший % яскравості встановлено, тим яскравіше світитиме джерело світла датчика кольору.

## Приклад

Приклад нижче встановлює яскравість світла для датчика кольору 75%.

```cpp
Color.setLight(75, percent);
```

<advanced>
</advanced>
