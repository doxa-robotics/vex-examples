category: sensing  
signature: Gyro.heading() 
device_class: gyro  
description: Reports the Gyro Sensor's current heading in degrees.

# Gyro Heading

Передає поточний курс гіродатчика у градусах.

```cpp
Gyro.heading()
```

## Як це працює

Команда `Gyro.heading` збільшує курс у напрямку **проти годинникової стрілки**.

`Gyro.heading` передає значення в діапазоні **від 0.00 до 359.99**.

## Приклад

Приклад нижче друкує курс гіродатчика на екрані VEX IQ Brain.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Gyro Heading: %.2f", Gyro.heading());

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>