category: looks  
signature: TouchLED.setFade(fade);  
device_class: led  
description: Sets the fade speed of the touchLED.

# Set TouchLED Fade

Визначає, як швидко відбудеться перехід між кольорами LED датчика дотику VEX IQ.

```cpp
TouchLED.setFade(fade);
```

## Як це працює

Перша частина команди - назва пристрою.

```cpp
TouchLED1.setFade(fast);
TouchLED2.setFade(slow);
```
Виберіть, як швидко відбудеться перехід LED датчика дотику.Замініть `fade` на одну з таких опцій:

* **slow** - LED датчик дотику повільно змінюватиме колір.
* **fast** - LED датчик дотику швидко змінюватиме колір.
* **off** - LED датчик дотику миттєво змінюватиме колір.

## Приклад

Цей приклад повільно змінить колір LED датчика дотику з червоного на синій.

```cpp
TouchLED.setColor(red);
TouchLED.setFade(slow);
TouchLED.setColor(blue);
```

<advanced>
</advanced>