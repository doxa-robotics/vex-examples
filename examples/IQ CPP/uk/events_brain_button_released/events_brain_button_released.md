category: events  
signature: Brain.button.released();  
description: Runs the callback function when the Brain’s touchscreen is released.  

# Brain Button Released

Запускає функцію зворотного виклику, коли відпущено кнопку VEX IQ Brain.

```cpp
Brain.Button.released(callback);
```

## Як це працює

Ви маєте створити функцію, яка буде викликатися, коли відпущено кнопку на  Brain.

```cpp
void buttonReleased() {
  Brain.Screen.print("Button released.");
}
```

Функцію `Brain.Button.released` можна використовувати з різними кнопками на VEX IQ Brain.

- `Brain.buttonUp.released(buttonReleased);`
- `Brain.buttonDown.released(buttonReleased);`
- `Brain.buttonCheck.released(buttonReleased);`

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Button.released(callbackFunction);
}
```

<advanced>
</advanced>