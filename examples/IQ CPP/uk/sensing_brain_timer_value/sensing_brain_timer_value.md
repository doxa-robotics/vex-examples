category: sensing  
signature: sensing_brain_timer_value
description: Reports the VEX IQ Brain's timer value in seconds. 

# Timer Value

Повертає значення таймера з VEX IQ Brain у секундах.

```cpp
Brain.Timer.value()
```

## Як це працює

Таймер починає відлік з 0 секунд, коли програма запускається, і передає десяткові значення (*double*).

## Приклад

Приклад нижче друкує значення таймера Brain.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Timer: %.2f", Brain.Timer.value());
  
  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>