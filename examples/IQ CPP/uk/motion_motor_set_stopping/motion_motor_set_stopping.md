category: motion  
signature: Motor.setStopping(brake);  
device_class: motor  
description: Sets the Motors brake mode.  

# Motor Set Stopping

Встановлює поведінку мотора VEX IQ під час зупинки.

```cpp
Motor.setStopping(brakeType);
```

## Як це працює

Перша частина команди - назва пристрою.

```cpp
ClawMotor.setStopping(brake);
ArmMotor.setStopping(hold);
```

Встановіть поведінку зупинки мотора:
- **brake** змушує мотор миттєво зупинитися.
- **coast** дає змогу мотору поступово зменшити оберти до зупинки.
- **hold** змушує мотор миттєво зупинитися і повертатиме його до позиції зупинки, якщо він зміститься.

Команда `Motor.setStopping` впливатиме на роботу всіх команд для мотора `Motor.stop` у цьому проєкті.

## Приклад

Цей приклад змусить мотор руки рухатися вгору 90 градусів, а потім миттєво зупинитися і компенсувати зовнішні сили (як-от гравітація), щоб утримувати позицію.

```cpp
ArmMotor.setStopping(hold);
ArmMotor.spinFor(forward, 90, degrees);
```

<advanced>
</advanced>