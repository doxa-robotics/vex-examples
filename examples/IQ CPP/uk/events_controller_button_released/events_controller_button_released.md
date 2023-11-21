category: events  
signature: Controller.Button.released();  
description: Runs the callback function when the Controller button is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.

# Controller Button Released

Запускає функцію зворотного виклику **callback function**, коли відпущено кнопку на контролері VEX IQ.

```cpp
Controller.Button.released(callback);
```

## Як це працює

Ви маєте створити функцію зворотного виклику (**callback function**), яка буде викликатися, коли кнопка на контролері відпущена.

```cpp
void buttonReleased() {
  Brain.Screen.print("Button released.");
}
```

Виберіть, яка кнопка контролера викличе функцію `released()`.

- `Controller.ButtonEUp.released(buttonReleased);`
- `Controller.ButtonEDown.released(buttonReleased);`
- `Controller.ButtonFUp.released(buttonReleased);`
- `Controller.ButtonFDown.released(buttonReleased);`
- `Controller.ButtonLUp.released(buttonReleased);`
- `Controller.ButtonLDown.released(buttonReleased);`
- `Controller.ButtonRUp.released(buttonReleased);`
- `Controller.ButtonRDown.released(buttonReleased);`

![controller_button_back](controller_button_front.jpg)


![controller_button_front](controller_button_back.png)

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Controller.ButtonRDown.released(callbackFunction);
}
```

<advanced>
</advanced>