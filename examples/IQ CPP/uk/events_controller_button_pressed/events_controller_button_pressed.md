category: events  
signature: Controller.Button.pressed();  
description: Runs the callback function when the Controller button is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.

# Controller Button Pressed

Запускає функцію зворотного виклику **callback function**, коли натиснуто кнопку на контролері VEX IQ.

```cpp
Controller.Button.pressed(callback);
```

## Як це працює

Ви маєте створити функцію зворотного виклику (**callback function**), яка буде викликатися, коли кнопка на контролері натиснута.

```cpp
void buttonPressed() {
  Brain.Screen.print("Button pressed.");
}
```

Виберіть, яка кнопка контролера викличе функцію `pressed()` .

![controller_button_back](controller_button_front.jpg)

- `Controller.ButtonEUp.pressed(buttonPressed);`
- `Controller.ButtonEDown.pressed(buttonPressed);`
- `Controller.ButtonFUp.pressed(buttonPressed);`
- `Controller.ButtonFDown.pressed(buttonPressed);`

![controller_button_front](controller_button_back.png)

- `Controller.ButtonLUp.pressed(buttonPressed);`
- `Controller.ButtonLDown.pressed(buttonPressed);`
- `Controller.ButtonRUp.pressed(buttonPressed);`
- `Controller.ButtonRDown.pressed(buttonPressed);`

<advanced>
</advanced>