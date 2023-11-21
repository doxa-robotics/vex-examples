category: drivetrain
signature: Drivetrain.setTurnVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain when turning. If this is used when the drivetrain is turning, the drivetrain will be updated with the new speed.  

# Set Turn Velocity

Встановлює швидкість поворотів трансмісії.

Якщо ця команда спрацьовує, коли трансмісія повертає, то трансмісія змінить свою швидкість на нову.

```cpp
Drivetrain.setTurnVelocity(velocity, units);
```

## Як це працює

`Drivetrain.setTurnVelocity` задає швидкість повороту трансмісії, але не запускає її рух.

`Drivetrain.setTurnVelocity` приймає значення в діапазоні **від -100 до 100**, коли використано одиниці **percent** - відсотки.

`Drivetrain.setTurnVelocity` иймає значення в діапазоні **від -127 до 127**, коли використано одиниці **rpm** - оберти за хвилину.

Встановлення швидкості повороту трансмісії у від'ємне значення змусить її повертати у зворотному напрямку.

Встановлення швидкості повороту трансмісії в 0 спричинить зупинку трансмісії.

## Приклад

Цей приклад змусить трансмісію повертати ліворуч зі швидкістю 25%.

```cpp
Drivetrain.setTurnVelocity(25, percent);
Drivetrain.turn(left);
```

<advanced>
</advanced>
