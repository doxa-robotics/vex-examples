category: sensing  
signature: Bumper.pressing()  
device-class: bumper
description: Reports if the VEX IQ Bumper is pressed.

# Bumper Pressing

Повідомляє, чи бамперний перемикач VEX IQ натиснуто.

```cpp
Bumper.pressing()
```

## Як це працює

`Bumper.pressing` передає значення **true**, якщо бамперний перемикач натиснуто.


`Bumper.pressing` передає значення **false**, якщо бамперний перемикач не натиснуто.

Перша частина команди - назва пристрою.

```cpp
Bumper2.pressing()
Bumper4.pressing()
```

## Приклад

Приклад нижче друкує на екрані Brain те, чи натиснуто бамперний перемикач.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Bumper Pressed: %s", Bumper2.pressing() ? "TRUE" : "FALSE");

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}
```

<advanced>
</advanced>
