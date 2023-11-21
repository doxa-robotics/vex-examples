category: events  
signature: TouchLED.released(callback);  
device_class: touchled  
description: Runs the specified callback function when the Touch LED is released.  

# TouchLED Released

Запускає функцію зворотного виклику **callback function**, коли датчик дотику TouchLED відпущено.

```cpp
TouchLED.released(callback);
```

## Як це працює

Ви маєте створити функцію, яка буде викликатися, коли датчик дотику відпущено. Назвіть цю функцію, яка має спрацювати в параметрі `callback` після виконання події.

```cpp
void touchLEDReleased() {
  Brain.Screen.print("Touch LED released.");
}
```
Потім, передайте цю функцію як параметр функції `TouchLED.released`.

```cpp
TouchLED.released(touchLEDReleased);
```

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**.

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  TouchLED.released(callbackFunction);
}
```

<advanced>
</advanced>