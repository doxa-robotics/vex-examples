category: control  
signature: wait(time, units);  
description: Waits for a specific amount of time before moving to the next command.  

# Wait

Очікує визначену кількість часу перед виконанням наступної команди.

```cpp
wait(time, units);
```

## Як це працює

Встановіть кількість часу в **seconds** (секундах) або **msec** (мілісекундах), щоб програма почекала - `wait` - перед виконанням наступних команд.

```cpp
wait(10, seconds);
wait(100, msec);
```

<advanced>
</advanced>