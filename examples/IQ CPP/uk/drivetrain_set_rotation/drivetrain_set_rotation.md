category: drive  
signature: Drivetrain.setHeading(90, degrees);  
device_class: smartdrive  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Set Drive Rotation

Встановлює значення кута повороту трансмісії, якщо налаштовано гіроскопічний датчик VEX IQ.

```cpp
Drivetrain.setRotation(rotation, degrees);
```
## Як це працює

Команду `Drivetrain.setRotation` використовують, щоб перезаписати поточну позицію кута повороту трансмісії на введене позитивне або негативне значення.

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