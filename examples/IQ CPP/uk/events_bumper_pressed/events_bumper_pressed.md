category: events  
signature: BUMPER.pressed(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is pressed.  

# Bumper Pressed

Запускає визначену функцію зворотного виклику **callback function**, коли натиснуто бампер.

```cpp
Bumper.pressed(callback);
```

## Як це працює

Ви маєте створити функцію, яка буде викликатися, коли натиснуто бамперний перемикач. Назвіть цю функцію, яка має спрацювати в параметрі `callback` після виконання події.

```cpp
void bumperPressed() {
  Brain.Screen.print("Bumper pressed.");
}
```
Потім, передайте цю функцію як параметр функції `Bumper.pressed`.

```cpp
Bumper.pressed(bumperPressed);
```

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**.

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Bumper.pressed(callbackFunction);
}
```

<advanced>
</advanced>