category: drive
signature: Drivetrain.setRotation(90, degrees);  
device_class: smartdrive  
description: Sets the Drivetrain's angle of rotation when configured with a VEX IQ Gyro Sensor.

# Set Rotation

Встановлює значення кута повороту трансмісії, якщо  налаштовано гіроскопічний датчик VEX IQ.


```cpp
Drivetrain.setRotation(value, rotationUnits);
```

## Як це працює

Команду `Drivetrain.setRotation()` використовують, щоб перезаписати поточну позицію кута повороту трансмісії на введене позитивне або негативне значення.

Команда `Drivetrain.setRotation()` приймає цілі, числові значення.

Команда `Drivetrain.setRoation()` **не** має обмежень у 0-359 градусів.

## Приклад

Цей приклад поверне робота на загальний кут 210 градусів:

```cpp
Drivetrain.turnToRotation(120, degrees);
Drivetrain.setRotation(-45, degrees);
Drivetrain.turnToRotation(45, degrees);
```

- Поворот ліворуч (проти годинникової стрілки) на 120 градусів.
- Встановлення поточної позиції кута повороту -45 градусів.
- Поворот ліворуч (проти годинникової стрілки) на додаткові 90 градусів (від -45 градусів до +45 градусів) через перевизначення кута в попередній команді.

<advanced>
</advanced>
