category: sensing  
signature: Brain.Button.pressing()  
description: Reports if a button on the VEX IQ Brain is pressed.

# Brain Button Pressing

Передає значення, якщо обрана кнопка на VEX IQ Brain натиснута.

```cpp
Brain.Button.pressing()
```

## Як це працює

Передає **true**, якщо обрана кнопка на Brain натиснута. Передає **false**, якщо обрана кнопка на Brain не натиснута.

Після частини команди `Brain.` введіть назву кнопки на Brain, яка буде реагувати на натискання.

Можливі варіанти кнопок на Brain:
- `buttonUp`
- `buttonDown`
- `buttonCheck`

## Приклад

Цей приклад змушує робота їхати вперед.

Потім, він перевіряє, чи натиснута кнопка **buttonUp**, і тоді повертає робота праворуч.

```cpp
Drivetrain.drive(forward);

while (true) {
  if (Brain.buttonUp.pressing()) {
    Drivetrain.turn(right);
    break;
  }

  wait(20, msec);
}
```

<advanced>
</advanced>