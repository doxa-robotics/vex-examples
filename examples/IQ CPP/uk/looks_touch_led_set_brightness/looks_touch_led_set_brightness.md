category: looks  
signature: TouchLED.brightness();  
device_class: led  
description: Sets the brightness of the touchLED.  

# Set TouchLED Brightness

Встановлює рівень яскравості LED датчика дотику VEX IQ.

```cpp
TouchLED.setBrightness(brightness);
```

## Як це працює

`TouchLED.setBrightness` приймає значення в діапазоні **від 0 до 100** для параметра яскравості `brightness`.

Перша частина команди - назва пристрою.

```cpp
TouchLED1.setBrightness(100);
TouchLED2.setBrightness(50);
```

## Приклад

Цей приклад змушує LED датчик дотику випромінювати зелене світло з яскравістю 25%.

```cpp
TouchLED.setBrightness(25);
TouchLED.setColor(green);
```

<advanced>
</advanced>