category: sensing  
signature: sensing_brain_timer_reset 
description: Resets the Brain's timer.

# Reset Timer

Скидає таймер VEX IQ Brain.

```cpp
Brain.Timer.reset();
```

## Як це працює

Таймер Brain починає відлік після старту кожного проєкта.  Команда `Brain.Timer.reset` скидає таймер до 0 секунд.

## Приклад

У цьому прикладі таймер буде скинуто, коли трансмісія проїде вперед упродовж 3 секунд. Коли мине 3 секунди, трансмісія зупиниться.

```cpp
Brain.Timer.reset();
Drivetrain.drive(forward);

while (true) {
  if (Brain.Timer.value() > 3) {
    break;
  }

  wait(20, msec);
}

Drivetrain.stop();
```

<advanced>
</advanced>