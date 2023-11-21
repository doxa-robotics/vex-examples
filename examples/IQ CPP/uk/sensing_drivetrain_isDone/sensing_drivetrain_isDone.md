category: sensing  
signature: Drivetrain.isDone()  
device_class: drivetrain  
description: Reports if the Drivetrain has completed its movement.

# Drive Is Done

Повідомляє, коли трансмісія закінчила рух.

```cpp
Drivetrain.isDone()
```

## Як це працює

`Drivetrain.isDone` передає значення **true**, коли мотори трансмісії закінчили свою роботу.

`Drivetrain.isDone` передає значення **false**, коли мотори трансмісії досі працюють.

## Приклад

Приклад нижче друкує на екрані VEX IQ Brain те, чи трансмісія закінчила свій рух.

```cpp
Drivetrain.driveFor(forward, 1000, mm, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain is Done: %s", Drivetrain.isDone() ? "TRUE" : "FALSE");

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>