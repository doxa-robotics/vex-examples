category: control  
signature: control_for
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# For

Повторює код всередині фігурних дужок встановлену кількість разів.

```cpp
for (initialization; condition; increment/decrement) {
  // якийсь код для повторювання
}
```

## Як це працює

Введіть значення, щоб визначити, скільки разів **повториться** код, використовуючи 3 параметри:

* оголошення
* умова
* інкремент/декремент

**Оголошення** задає початкове значення ітеративної змінної.

**Умова** визначає, як довго працюватиме цикл for. Цикл припинить повторюватися, коли значення умови стане **false**.

**Інкремент/декремент** змінює значення ітеративної змінної наприкінці кожного виконаного циклу.

## Приклад 1

Цей приклад надрукує числа від 0 до 9 на екрані VEX IQ Brain.

```cpp
for (int i = 0; i < 10; i++) {
  Brain.Screen.print("%d", i);
  wait(20, msec);
}
```
## Приклад 2

Цей приклад запустить робота VEX IQ вперед на 250 мм, а потім поверне його праворуч на 60 градусів тричі.

```cpp
Drivetrain.driveFor(forward, 250, mm);

for (int i = 0; i < 3; i++) {
  Drivetrain.turnFor(right, 60, degrees);
  wait(20, msec);
}
```

<advanced>
</advanced>