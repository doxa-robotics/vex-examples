category: sensing  
signature: Color.hue()  
device-class: colorsensor
description: Reports the hue of the color detected by the VEX IQ Color Sensor.

# Color Hue

Передає відтінок кольору, який побачив датчик кольору VEX IQ.

```cpp
Color.hue()
```

## Як це працює

`Color.hue` передає значення в діапазоні **від 0 до 360** градусів, що представляє позицію кольору на колі кольорів.

## Приклад

Приклад друкує відтінок кольору, який побачив датчик кольору.

```cpp
Brain.Screen.print("Hue: %.0f", Color.hue());
```

<advanced>
</advanced>