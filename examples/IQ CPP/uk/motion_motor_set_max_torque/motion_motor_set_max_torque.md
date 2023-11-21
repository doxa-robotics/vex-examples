category: motion  
signature: Motor.setMaxTorque(50, percent);
device_class: motor  
description: Sets the Motor's max torque.  

# Motor Set Max Torque

Встановлює максимальну силу обертання мотора.

```cpp
Motor.setMaxTorque(value, percent);
```

## Як це працює

`Motor.setMaxTorque` приймає значення в діапазоні **від 0% до 100%**.

Перша частина команди - назва пристрою.

```cpp
ClawMotor.setMaxTorque(25, percent);
ArmMotor.setMaxTorque(75, percent);
```

## Приклад

Цей приклад обертатиме ClawMotor в позицію 40 градусів із крутним моментом 20%. Це дасть змогу клешні схопити об'єкт без пошкоджень від надмірного стиснення.

```cpp
ClawMotor.setMaxTorque(20, percent);
ClawMotor.spinToPosition(40, degrees);
```

<advanced>
</advanced>