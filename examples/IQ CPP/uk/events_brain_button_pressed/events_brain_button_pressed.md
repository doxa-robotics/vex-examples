category: events  
signature: Brain.buttonUp.pressed(callback);  
description: Runs the callback function when the Brain’s touchscreen is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Brain Button Pressed

Запускає функцію зворотного виклику, коли натиснуто кнопку VEX IQ Brain.

```cpp
Brain.Button.pressed(callback);
```

## Як це працює

Ви маєте створити функцію, яка буде викликатися, коли натиснути кнопку на  Brain.

```cpp
void buttonPressed() {
  Brain.Screen.print("Button pressed.");
}
```

Функцію `Brain.Button.pressed` можна використовувати з різними кнопками на VEX IQ Brain.

- `Brain.buttonUp.pressed(buttonPressed);`
- `Brain.buttonDown.pressed(buttonPressed);`
- `Brain.buttonCheck.pressed(buttonPressed);`

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Button.pressed(callbackFunction);
}
```

<advanced>
</advanced>