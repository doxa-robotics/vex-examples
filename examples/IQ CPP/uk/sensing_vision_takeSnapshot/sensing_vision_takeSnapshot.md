category: sensing  
signature: Vision.takeSnapshot(signature);  
device_class: vision  
description: Takes a snapshot from the Vision Sensor. A user defined signature or color code will need to replace the "SIGNATURE" parameter in order for this example snippet to compile.

# Vision Take Snapshot

Робить знімок датчиком зору.

```cpp
Vision.takeSnapshot(signature);
```

## Як це працює

`Vision.takeSnapshot` фіксує поточне зображення з датчика зору, щоб обробити і проаналізувати його на сигнатури кольору та коди.

Перед використанням команди `Vision.takeSnapshot` треба налаштувати датчик зору хоча б на одну сигнатуру. Ім'я сигнатури буде згенеровано автоматично.

Наприклад, якщо назва датчика `Vision1`, а сигнатура налаштована з ім'ям `REDBOX`, ім'я сигнатури буде `Vision1__REDBOX`, і для створення знімка треба викликати:

```cpp
Vision1.takeSnapshot(Vision1__REDBOX);
```

Зазвичай, `Vision.takeSnapshot` треба викликати перед використанням інших команд датчика зору.

Переконайтеся, що правильно назвали датчик зору і сигнатуру, коли використовуватимете цю команду. Сигнатуру датчика зору можна налаштувати з вікна налаштувань робота.

<advanced>
</advanced>