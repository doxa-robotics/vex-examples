category: motion  
signature: Motor.spin(forward);  
device_class: motor  
description: Spins a Motor in a direction until stopped.  

# Spin Motor

Обертає мотор VEX IQ в певному напрямку.

```cpp
Motor.spin(direction);
```

## Як це працює

Команда `Motor.spin` постійно крутитиме мотор, поки не запрацює інший блок мотору або програма не зупиниться.

- **forward** обертає мотор вперед.
- **reverse** обертає мотор зворотно.

```cpp
Motor.spin(forward);
Motor.spin(reverse);
```

<advanced>
</advanced>