category: sensing  
signature: Color.isNearObject()  
description: Reports if the Color Sensor is near an object.

# Color Is Near Object

Повідомляє, якщо датчик кольору VEX IQ знайшов об'єкт або поверхню.

```cpp
Color.isNearObject()
```

## Як це працює

Перша частина команди - назва пристрою.

```cpp
Color5.isNearObject()
Color7.isNearObject()
```

Передає значення **true** , коли датчик кольору бачить перешкоду або поверхню попереду датчика.

Передає значення **false**, коли датчик кольору бачить пустий простір попереду датчика.

## Приклад

Приклад нижче друкує, чи побачив датчик кольору об'єкт або поверхню.

```cpp
Brain.Screen.print("Is Near Object: %s", Color.isNearObject() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>