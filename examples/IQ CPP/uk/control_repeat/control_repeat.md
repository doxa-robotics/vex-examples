category: control  
signature: repeat(10) { }  
description: Repeats the code inside curly brackets for a set number of times.

# Repeat

Повторює команди всередині фігурних дужок задану в круглих дужках кількість разів.
`repeat (number of times to repeat){code to repeat}`

```
repeat (10) {

}
```

## Як це працює

**Оператор repeat** циклічно виконуватиме код всередині фігурних дужок, поки не досягне встановленої в умові кількості виконань.

Спершу, задайте кількість разів, яку код повторюватиметься, вписавши в умову додатне ціле число. Умова може бути змінною або даними з датчиків.

Фрагмент нижче надрукує "iteration" на екрані Brain чотири рази. Щоразу він створюватиме новий рядок перед друкуванням наступної ітерації.

```
repeat (4) {
  Brain.Screen.print("iteration");
  Brain.Screen.newLine();
  wait(5, msec);
}
```

Зверніть увагу, що **оператор repeat** не можна розміщувати в іншому операторі repeat.

<advanced>
</advanced>