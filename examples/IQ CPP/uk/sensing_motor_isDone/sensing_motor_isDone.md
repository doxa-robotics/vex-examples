category: sensing  
signature: Motor.isDone()  
device_class: motor  
description: Reports if the Motor has completed its movement.

# Motor Is Done

Повідомляє, якщо вибраний мотор зупинився.

```cpp
Motor.isDone()
```

## Як це працює

`Motor.isDone` передає значення  **true**, коли вибраний мотор закінчив свою роботу.

`Motor.isDone` передає значення  **false**, коли вибраний мотор досі працює.

## Приклад

Приклад нижче друкує на екрані VEX IQ Brain те, чи мотор ArmMotor закінчив свій рух.

```cpp
ArmMotor.spinFor(forward, 270, degrees, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("ArmMotor is Done: %s", ArmMotor.isDone() ? "TRUE" : "FALSE");

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>