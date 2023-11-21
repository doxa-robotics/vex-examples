category: sensing  
signature: Gyro.rotation()  
device_class: gyro  
description: Reports the Gyro Sensor's current rotation in degrees.

# Gyro Rotation

Передає поточний кут повороту гіродатчика VEX IQ у градусах.

```cpp
Gyro.rotation()
```

## Як це працює

`Gyro.rotation` збільшує значення, коли гіродатчик обертається у напрямку **проти годинникової стрілки**.

`Gyro.rotation` зменшує значення, коли гіродатчик обертається у напрямку **за годинниковою стрілкою**.

## Приклад

Приклад нижче друкує кут повороту гіродатчика на екрані VEX IQ Brain.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Gyro Rotation: %.2f", Gyro.rotation());

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>