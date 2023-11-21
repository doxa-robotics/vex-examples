category: sensing  
signature: Distance.foundObject()  
device-class: sonar
description: Reports if the VEX IQ Distance Sensor sees an object within its field of view. 

# Distance Found Object

Повідомляє, якщо датчик відстані VEX IQ бачить об'єкт у полі зору.

```cpp
Distance.foundObject()
```

## Як це працює

Передає значення **true**, коли датчик відстані бачить об'єкт або перешкоду в полі зору. Передає значення **false**, коли датчик відстані не бачить об'єктів або перешкод.

Перша частина команди - назва пристрою.

```cpp
Distance3.foundObject()
Distance4.foundObject()
```

## Приклад

Приклад нижче друкує, чи бачить датчик відстані об'єкт або поверхню в полі зору.

```cpp
Brain.Screen.print("Found Object: %s", Distance.foundObject() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>