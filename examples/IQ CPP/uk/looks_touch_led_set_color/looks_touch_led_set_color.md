category: looks  
signature: touchLED.color();  
device_class: led  
description: Sets the color of the touchLED.  

# Set TouchLED Color

Встановлює колір для LED датчика дотику VEX IQ.

```cpp
TouchLED.setColor(color);
```

## Як це працює

Перша частина команди - назва пристрою.

```cpp
TouchLED1.setColor(red);
TouchLED2.setColor(green);
```
Виберіть колір світіння.

Варіанти кольору:

- `red`
- `green`
- `blue`
- `white`
- `yellow`
- `orange`
- `purple`
- `red_violet`
- `violet`
- `blue_violet`
- `blue_green`
- `yellow_green`
- `yellow_orange`
- `red_orange`

Щоб вимкнути колір LED датчика дотику, встановіть колір **colorType::none**.

```cpp
TouchLED.setColor(colorType::none);
```

<advanced>
</advanced>