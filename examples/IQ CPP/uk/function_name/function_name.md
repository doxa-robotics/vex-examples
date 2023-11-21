category: functions  
signature: function_name
device_class: function  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Functions

Функції - це частини коду, які використовують для виконання набору дій. 

```cpp
void myFunction() {
  // код функції
}
```

## Як це працює

Щоб визначити функцію, оголосіть тип даних, які функція повертатиме.

- `int`, `float`, `double`, і `string` - типи даних, які повертають найчастіше. Якщо функція не має повертати значення, оголосіть тип даних `void`.

Потім, назвіть функцію зрозумілим ім'ям, яке описує те, що функція робить.

```cpp
int returnZero() {
  return 0;
}
```

Додайте дужки `()` з необов'язковими *параметрами* після імені функції. Декілька параметрів треба розділяти комами (параметр1, параметр2).

Тіло функції треба помістити у фігурні дужки `{ }`.
    
## Приклад

Ця функція не має параметрів і не повертає значень, тому її тип (або тип даних, які вона повертає) оголошено `void`. Ця функція друкує "The battery is low!" на екрані VEX IQ Brain, якщо заряд батареї нижче 25%.

```cpp
void lowOnBattery() {
  if (Brain.Battery.capacity(percent) < 25.0) {
    Brain.Screen.print("The battery is low!");
  }
}
```

<advanced>
</advanced>