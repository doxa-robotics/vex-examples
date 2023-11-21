category: motion  
signature: Motor.setPosition(0, degrees);  
device_class: motor  
description: Sets the Motor's encoder to a position.  

# Motor Set Position

Встановлює значення позиції енкодера мотора VEX IQ на введену величину.

```cpp
Motor.setPosition(position, units);
```

## Як це працює

Команду `Motor.setPosition` використовують, щоб перезаписати поточну позицію мотора на задане значення.

Перша частина команди - назва пристрою.

```cpp
ClawMotor.setPosition(0, degrees);
ArmMotor.setPosition(90, degrees);
```

Зазвичай, команду `Motor.setPosition` використовують, щоб скинути позицію енкодера мотора в 0.

Встановіть одиниці вимірювання `units` **degrees** або **turns**.

## Приклад

Цей приклад встановить позицію мотора ClawMotor в 50 градусів.

```cpp
ClawMotor.setPosition(50, degrees);
```

<advanced>
</advanced>