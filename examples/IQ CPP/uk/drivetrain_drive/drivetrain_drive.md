category: drive  
signature: Drivetrain.drive(forward);  
device_class: drivetrain  
description: Moves the Drivetrain forever. All drivetrain motors are run forwards or backwards at the speed that was set using `Drivetrain.setDriveVelocity`, the default speed is 50 rpm.

# Drive

Рухає трансмісію вперед.

```cpp
Drivetrain.drive(direction);
```

Всі мотори трансмісії запускаються вперед або назад зі швидкістю, встановленою командою `Drivetrain.setDriveVelocity`. Швидкість за замовчуванням 50 rpm (об/хв).

## Як це працює

Команда `Drivetrain.drive` постійно рухатиме трансмісію, поки не запрацює нова команда трансмісії або програма не зупиниться.

Використайте параметр **forward**, щоб запустити трансмісію на рух уперед.

```cpp
Drivetrain.drive(forward);
```

Використайте параметр **reverse**, щоб запустити трансмісію у зворотному напрямку.

```cpp
Drivetrain.drive(reverse);
```
 
<advanced>
</advanced>