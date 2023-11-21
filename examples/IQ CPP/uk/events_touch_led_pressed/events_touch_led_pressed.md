category: events  
signature: TouchLED.pressed(callback);  
device_class: TouchLED  
description: Runs the specified callback function when the Touch LED is pressed.  

# TouchLED Pressed

Запускає функцію зворотного виклику **callback function**, коли датчик дотику TouchLED натиснуто.

```cpp
TouchLED.pressed(callback);
```

## Як це працює

Ви маєте створити функцію, яка буде викликатися, коли датчик дотику натиснуто. Назвіть цю функцію, яка має спрацювати в параметрі `callback` після виконання події.

```cpp
void touchLEDPressed() {
  Brain.Screen.print("Touch LED pressed.");
}
```
Потім, передайте цю функцію як параметр функції `TouchLED.pressed`.

```cpp
TouchLED.pressed(touchLEDPressed);
```

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  TouchLED.pressed(callbackFunction);
}
```

<advanced>
</advanced>