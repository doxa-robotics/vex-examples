category: control  
signature: control_if
description: Runs the code inside the if-statement's curly brackets, if the condition returns true. 

# If

Виконує код всередині фігурних дужок оператора if, якщо умова повертає true. 

```cpp
if (condition) {
  // код, який виконається, якщо умова true
}
```

## Як це працює

**Оператор if** перевіряє свою умову в круглих дужках лише один раз.

Якщо умова повертає **true**, код всередині фігурних дужок виконається.

Якщо умова повертає **false**, код всередині фігурних дужок буде пропущено.

```cpp
// Зупинити Motor1, якщо  BumperA натиснуто
if (BumperA.pressing()) {
  Motor1.stop();
}
```

<advanced>
</advanced>