category: drive  
signature: Drivetrain.stop();  
device_class: drivetrain  
description: Stops the Drivetrain.  

# Stop

Зупиняє трансмісію.

```cpp
Drivetrain.stop();
```

## Як це працює

Команда `Drivetrain.stop` змушує трансмісію зупинитися.

Режим гальмування можна встановити командою `Drivetrain.setStopping`.

## Приклад

Цей приклад запустить робота VEX IQ на рух вперед на 3 секунди, а потім зупинить його.

```cpp
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>