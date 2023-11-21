category: drive  
signature: Drivetrain.setTimeout(1, seconds);  
device_class: drivetrain  
description: Sets the timeout for the Drivetrain to stop moving if a blocking command cannot reach its target.  

# Set Timeout

Часові обмеження руху трансмісії потрібні, щоб команди руху, які не змогли досягти своєї позиції, не заважали працювати наступним командам.

```cpp
Drivetrain.setTimeout(time, seconds);
```

## Як це працює

Команда `Drivetrain.setTimeout` використовується, щоб команди руху, які не виконалися, не блокували роботу інших команд.

Приклад трансмісії, яка не досягла своєї позиції - коли під час руху робот зіткнувся зі стіною і не може закінчити свій рух.

Встановіть часові обмеження тривалості руху, вказавши кількість часу в секундах - `seconds`.

```cpp
Drivetrain.setTimeout(2.0, seconds);
```

## Приклад

Цей приклад зупинить команду `Drivetrain.driveFor` через дві секунди, якщо трансмісія не встигне проїхати 600 міліметрів.

Щойно часові обмеження або відстань будуть подолані (залежить від того, що раніше), трансмісія поверне праворуч на 90 градусів.

```cpp
Drivetrain.setTimeout(2.0, seconds);
Drivetrain.driveFor(forward, 600, mm);
Drivetrain.turnFor(right, 90.0, degrees);
```

<advanced>
</advanced>