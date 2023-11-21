category: sensing  
signature: Drivetrain.isMoving()  
device_class: drivetrain  
description: Reports if the Drivetrain is currently moving.

# Drive Is Moving

Повідомляє, якщо трансмісія рухається.

```cpp
Drivetrain.isMoving()
```

## Як це працює

Ця команда передає значення **true**, якщо трансмісія рухається внаслідок роботи команди `Drivetrain.driveFor` або `Drivetrain.turnFor`, які мають встановлену відстань руху.

Ця команда передає значення **false**, якщо трансмісія закінчила рух.

**Зауваження:** Ця команда завжди повертає **false**, якщо виконуються команди `Drivetrain.drive` або `Drivetrain.turn` (вони *не* мають встановленої відстані руху).

## Приклад

Приклад нижче друкує на екрані VEX IQ Brain те, чи трансмісія ще рухається.

```cpp
Drivetrain.driveFor(forward, 1000, mm, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain is Moving: %s", Drivetrain.isMoving() ? "TRUE" : "FALSE");

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>