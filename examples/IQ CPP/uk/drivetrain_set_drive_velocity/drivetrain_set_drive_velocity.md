category: drivetrain
signature: Drivetrain.setDriveVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain that will be used for drive and driveFor calls. If this is used when the drive is moving, the drivetrain will be updated with the new speed. 

# Set Drive Velocity

Встановлює швидкість руху трансмісії для команд `Drivetrain.drive` і `Drivetrain.driveFor`. 

Якщо ця команда спрацьовує, коли трансмісія рухається, то трансмісія змінить свою швидкість на нову.

```cpp
Drivetrain.setDriveVelocity(velocity, units);
```

## Як це працює

`Drivetrain.setDriveVelocity` задає швидкість трансмісії, але не запускає її рух.

`Drivetrain.setDriveVelocity` приймає значення в діапазоні **від -100 до 100**, коли використано одиниці **percent** - відсотки.

`Drivetrain.setDriveVelocity` приймає значення в діапазоні **від -127 до 127**, коли використано одиниці **rpm** - оберти за хвилину.

Встановлення швидкості трансмісії у від'ємне значення змусить її працювати у зворотному напрямку.

Встановлення швидкості трансмісії в 0 спричинить зупинку трансмісії.

## Приклад

Цей приклад змусить трансмісію проїхати 300 міліметрів зі швидкістю 50%.

```cpp
Drivetrain.setDriveVelocity(50, percent);
Drivetrain.driveFor(forward, 30, mm);
```

<advanced>
</advanced>
