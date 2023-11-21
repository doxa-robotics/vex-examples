category: sensing  
signature: Drivetrain.heading(degrees)  
description: Reports the Drivetrain's heading.

# Drive Heading

Передає напрямок у який спрямована трансмісія.

```cpp
Drivetrain.heading(degrees)
```

## Як це працює

`Drivetrain.heading` передає значення в діапазоні **від 0.00 до 359.99 градусів**.

## Приклад

Приклад нижче друкує курс трансмісії на екрані VEX IQ Brain.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain Heading: %.2f", Drivetrain.heading(degrees));

    // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>
