category: drive 
signature: Drivetrain.turnToRotation(90, degrees);  
device_class: smartdrive  
description: Turns a Drivetrain to a specific angle of rotation when configured with a VEX IQ Gyro Sensor.

# Turn To Rotation

Повертає трансмісію на визначений кут, якщо налаштовано гіроскопічний датчик VEX IQ.

```cpp
Drivetrain.turnToRotation(rotation, degrees);
```

## Як це працює

Команду `Drivetrain.turnToRotation` використовують, щоб повернути трансмісію на введене позитивне (проти годинникової стрілки) або негативне (за годинниковою стрілкою) значення.

Зважаючи на поточний кут повороту трансмісії, `Drivetrain.turnToRotation` самостійно обере напрямок обертання.

Параметр `rotation` **не** обмежується діапазоном **від 0 до 359.99 градусів**. Повороти будуть повними і можуть повернути робота більш ніж на один оберт, якщо потрібно.

## Приклад

Цей приклад змусить трансмісію здійснити чотири повороти:

```cpp
Drivetrain.turnToRotation(90.0, degrees);
Drivetrain.turnToRotation(180, degrees);
Drivetrain.turnToRotation(-45, degrees);
Drivetrain.turnToRotation(0, degrees);
```

- Ліворуч (проти годинникової) до 90 градусів
- Ліворуч (проти годинникової) до 180 градусів
- Праворуч (за годинниковою) до -45 градусів
- Ліворуч (проти годинникової) до 0 градусів

Команда `Drivetrain.turnToRotation` за замовчуванням блокує інші команди, поки трансмісія повертає.

## Необов'язкові параметри

Ви можете встановити значення останнього параметра `false`, щоб команда `Drivetrain.turnToRotation` не блокувала програму під час виконання руху.

```cpp
Drivetrain.turnToRotation(180.0, degrees, false);
```

<advanced>
</advanced>
