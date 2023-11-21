category: drive  
signature: Drivetrain.setHeading(90, degrees);  
device_class: smartdrive  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Set Heading

Встановлює значення курсу гіроскопа трансмісії.

```cpp
Drivetrain.setHeading(heading, degrees);
```

## Як це працює

Команду `Drivetrain.setHeading` використовують, щоб перезаписати поточну позицію курсу трансмісії. 

`Drivetrain.setHeading` приймає позицію в діапазоні **від 0 до 359.99** для параметра `heading`.

## Приклад 

Цей приклад поверне робота на загальний кут 135 градусів.

```cpp
Drivetrain.turnToHeading(45.0, degrees);
Drivetrain.setHeading(0.0, degrees);
Drivetrain.turnToHeading(90.0, degrees);
```
- Поворот ліворуч на курс 45 градусів.
- Встановлення поточної позиції курсу робота 0 градусів.
- Поворот ліворуч на додаткові 90 градусів, оскільки позиція курсу в попередній команді була перевизначена.

<advanced>
</advanced>
