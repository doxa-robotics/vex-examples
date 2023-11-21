category: control  
signature: control_break
description: Exits a repeating loop immediately.

# Break

Негайно виходить із повторюваного циклу.

```cpp
break;
```

## Як це працює

Якщо її додати в цикл, команда `break` вийде з циклу в момент виконання.

## Приклад

Цей приклад запускає трансмісію вперед і перевіряє, чи натиснута кнопка Вгору на VEX IQ Brain.

Якщо кнопку Вгору натиснути, команда `break` вийде з циклу `while` і зупинить трансмісію.

```cpp
while (true) {
  Drivetrain.drive(forward);
  if (Brain.buttonUp.pressing()) {
    break;
  }
  wait(20, msec);
}

Drivetrain.stop();
```
<advanced>
</advanced>
