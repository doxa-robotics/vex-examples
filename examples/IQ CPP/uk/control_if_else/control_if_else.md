category: control  
signature: control_if_else
description: Runs the code inside the else-statement's curly brackets, if the if-statement's condition is false. This command must have an if-statement preceding for it to compile.  

# If/else

Оператор керування, який виконає код всередині першої або другої пари фігурних дужок залежно від того, яке логічне значення умови.

```cpp
if (condition) {
  // Цей код виконається, якщо умова поверне true
} else {
  // Цей код виконається, якщо умова поверне false
}
```

## Як це працює

Оператор if/else перевіряє значення логічної умови лише один раз.

Якщо логічна умова `(condition)` повертає **true**, код всередині фігурних дужок `if` виконається.

Якщо логічна умова `(condition)` повертає **false**, код всередині фігурних дужок `else` виконається.

## Приклад

У цьому прикладі LED датчик дотику VEX IQ засвітиться зеленим, якщо на нього натиснути, і засвітиться червоним, якщо ні.

Умову if/else можна “вкласти” або розмістити всередині циклу while, щоб LED датчик дотику перемикав колір більше, ніж один раз.

```cpp
while (true) {
  if (TouchLED.pressing()) {
    TouchLED.setColor(green);
  } else {
    TouchLED.setColor(red);
  }

  wait(20, msec);
}
```

<advanced>
</advanced>