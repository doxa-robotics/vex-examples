category: sensing  
signature: Color.detects(color)  
device-class: colorsensor
description: Reports if a color sensor detects a specific color.

# Color Detects

Повідомляє, якщо датчик кольору VEX IQ побачив певний колір.

```cpp
Color.detects(color)
```

## Як це працює

Передає значення  **true**, якщо датчик кольору побачив обраний колір. Передає значення **false** якщо датчик кольору побачив колір, не схожий на обраний.

Перша частина команди - назва пристрою.

```cpp
Color1.detects(red)
Color2.detects(blue)
```

Виберіть, який колір шукати:

- `red`
- `orange`
- `yellow`
- `green`
- `blue`
- `purple`
- `violet`
- `red_violet`
- `blue_violet`
- `blue_green`
- `yellow_green`
- `yellow_orange`
- `red_orange`
- `white`

Ви також можете передати **colorType::none** у параметр `color`, щоб дізнатись, що датчик кольору **не** знайшов об'єкт.

## Приклад

Цей приклад надрукує "Color Red" або "Other Color" залежно від того, побачив датчик кольору червоний, чи ні.

```cpp
if (Color.detects(red)) { 
  Brain.Screen.print("Color Red");
} else {
  Brain.Screen.print("Other Color");
}
```

<advanced>
</advanced>