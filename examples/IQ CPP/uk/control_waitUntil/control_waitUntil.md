category: control  
signature: control_waitUntil 
description: Waits for a condition to return true before moving to the next command.

# Wait Until

Повторює частину коду, поки задана **умова** не поверне **true**.

```cpp
while (!condition) { 
  // Код повторюватиметься, поки умова не поверне true
}
```

## Як це працює

Цей оператор керування постійно перевірятиме свою умову і **не** виконуватиме свій код, поки умова повертає **true**. Він може повторити весь код у фігурних дужках.

```cpp
while (!TouchLED.pressing()) {
  wait(20, msec);
}
```

## Приклад 

Цей приклад вмикає жовтий колір LED датчика дотику і чекає, поки на нього не натиснуть. Щойно натиснуть, LED датчик дотику змінить колір на зелений.

```cpp
TouchLED.setColor(yellow);

while (!TouchLED.pressing()) {
  wait(1, seconds);
}

TouchLED.setColor(green);
```

<advanced>
</advanced>