category: drive  
signature: Drivetrain.turn(right);  
device_class: drivetrain  
description: Turns the Drivetrain.  

# Turn

Повертає трансмісію.

```cpp
Drivetrain.turn(direction);
```

## Як це працює

Команда `Drivetrain.turn` постійно повертатиме трансмісію, поки не запрацює нова команда трансмісії або програма не зупиниться.

Використовуйте аргумент **left**, щоб повертати трансмісію ліворуч.

```cpp
Drivetrain.turn(left);
```

Використовуйте аргумент **right**, щоб повертати трансмісію праворуч.

```cpp
Drivetrain.turn(right);
```

<advanced>
</advanced>
