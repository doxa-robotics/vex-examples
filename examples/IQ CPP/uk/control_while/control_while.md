category: control  
signature: control_while
description: A loop that repeats the code inside the curly brackets while the condition returns true. 

# While

Цикл, який повторює код всередині, поки **умова** має результат **true**.   

```cpp
while (condition) {
  // Код повторюватиметься, поки умова повертає true
}
```

## Як це працює

Цикл `while` перевіряє значення умови в круглих дужках на початку кожного циклу.

Якщо умова повертає значення **true**, код всередині `while` виконається.

Якщо умова повертає значення **false**, код всередині `while` буде пропущено.

Цикл `while` приймає у свою умову все, що може мати значення **true** або **false**. Умови можуть бути булевими (логічними) або результатом порівнянь чи логічних операторів.

## Приклад

Цей приклад запустить робота VEX IQ вперед, поки значення таймера менше 60 секунд.

Через 60 секунд робот зупиниться.

```cpp
while(Brain.Timer.value() < 60) {
  Drivetrain.drive(forward);
  wait(20, msec);
}

Drivetrain.stop();
```

<advanced>
</advanced>