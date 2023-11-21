category: Events
signature: `Controller.AxisA.changed(callback)`  
device_class: Controller
description: Runs callback funtion when the selected VEX IQ Controller joystick axis is moved.

# Controller Axis Changed

Запускає функцію зворотного виклику, коли вибрана вісь джойстиків контролера VEX IQ рухається.

```cpp
Controller.Axis.changed(callback);
```

## Як це працює

Ви маєте створити функцію зворотного виклику, яка буде викликатися, коли вісь на контролері рухається.

```cpp
void axisMoved() {
  Brain.Screen.print("Axis moved.");
}
```

Виберіть, яку вісь джойстиків контролера використати і передайте функцію зворотного виклику

- `Controller.AxisA.changed(axisMoved);`
- `Controller.AxisB.changed(axisMoved);`
- `Controller.AxisC.changed(axisMoved);`
- `Controller.AxisD.changed(axisMoved);`

![controller_button_front](controller_button_front.jpg)

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Controller.AxisA.changed(callbackFunction);
}
```

<advanced>
</advanced>