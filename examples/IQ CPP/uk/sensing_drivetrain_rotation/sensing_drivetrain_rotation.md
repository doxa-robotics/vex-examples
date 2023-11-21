category: sensing  
signature: Drivetrain.rotation(degrees)  
device-class: drivetrain
description: Reports the Drivetrain's angle of rotation in degrees when configured with a VEX IQ Gyro Sensor.

# Drive Rotation

Передає кут повороту трансмісії у градусах.

```cpp
Drivetrain.rotation(degrees)
```

## Як це працює

`Drivetrain.rotation` збільшує і передає значення, коли трансмісія повертає у напрямку **проти годинникової стрілки**.

`Drivetrain.rotation` зменшує і передає значення, коли трансмісія повертає у напрямку **за годинниковою стрілкою**.

## Приклад

Приклад нижче друкує кут повороту трансмісії на екрані VEX IQ Brain.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain Rotation: %.2f", Drivetrain.rotation(degrees));

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>