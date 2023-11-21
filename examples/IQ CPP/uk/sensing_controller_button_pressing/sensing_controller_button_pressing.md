category: sensing  
signature: Controller.Button.pressing()  
device_class: controller  
description: Reports if a button on the Controller is pressed.

# Controller Button Pressing

Повідомляє, якщо обрана кнопка на контролері VEX IQ натиснута.

```cpp
Controller.Button.pressing()
```

## Як це працює

Виберіть, яка кнопка на контролері реагуватиме на натискання.

![controller_button_back](controller_button_front.jpg)

- `Controller.ButtonEUp.pressing()`
- `Controller.ButtonEDown.pressing()`
- `Controller.ButtonFUp.pressing()`
- `Controller.ButtonFDown.pressing()`

![controller_button_front](controller_button_back.png)

- `Controller.ButtonLUp.pressing()`
- `Controller.ButtonLDown.pressing()`
- `Controller.ButtonRUp.pressing()`
- `Controller.ButtonRDown.pressing()`

`Controller.Button.pressing()` передає значення **true**, якщо вибрана кнопка контролера натиснута.

`Controller.Button.pressing()` передає значення **false**, якщо вибрана кнопка контролера не натиснута.

## Приклад

Цей приклад нижче запускає робота VEX IQ вперед. Якщо натиснути кнопку ButtonEUp, робот зупиниться.

```cpp
Drivetrain.drive(forward);

while (true) {
  if (Controller.ButtonEUp.pressing()) {
    Drivetrain.stop();
    break;
  }

  wait(20, msec);
}

```

<advanced>
</advanced>