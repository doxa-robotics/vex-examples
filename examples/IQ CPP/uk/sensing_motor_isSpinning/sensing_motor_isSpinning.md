category: sensing  
signature: Motor.isSpinning()  
device_class: motor  
description: Reports if the selected Motor is currently spinning.

# Motor Is Spinning

Повідомляє, якщо вибраний мотор зараз обертається.

```cpp
Motor.isSpinning()
```

## Як це працює

Ця команда передає значення **true**, коли вибраний мотор обертається.

Ця команда передає значення **false**, коли вибраний мотор зупинено.

**Зауваження:** Ця команда завжди повертає **false**, якщо мотор обертається внаслідок виконання команди `Motor.spin` (вона *не* має встановленого кута повороту).

## Приклад

Приклад нижче надрукує на екрані VEX IQ Brain, чи обертається мотор ArmMotor.

```cpp
ArmMotor.spinFor(forward, 270, degrees, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("ArmMotor is Spinning: %s", ArmMotor.isSpinning() ? "TRUE" : "FALSE");

  //Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>