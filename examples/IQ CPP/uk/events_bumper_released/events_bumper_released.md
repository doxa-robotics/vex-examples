category: events  
signature: Bumper.released(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Bumper Released

Запускає визначену функцію, коли бампер відпущено.

```cpp
Bumper.released(callback);
```

## Як це працює

Ви маєте створити функцію, яка буде викликатися, коли бамперний перемикач відпущено. Назвіть цю функцію, яка має спрацювати в параметрі `callback` після виконання події.

```cpp
void bumperReleased() {
  Brain.Screen.print("Bumper released.");
}
```
Потім, передайте цю функцію як параметр функції `Bumper.released`.

```cpp
Bumper.released(bumperReleased);
```

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Bumper.released(callbackFunction);
}
```

<advanced>
</advanced>