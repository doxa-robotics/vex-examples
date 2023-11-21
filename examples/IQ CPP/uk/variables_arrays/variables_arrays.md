category: variables  
signature: variables_arrays
description: Declares the type, name, length of an array. 

# Array Variables

Оголошує тип, ім'я, довжину масиву.

```cpp
int myArray[3] = { 1, 2, 3 };
```

## Як це працює

Оголосіть, який тип даних зберігатиметься у вашому масиві. 

- `int`
- `double`
- `bool`

Назвіть масив характерним та унікальним ім'ям. Встановіть розміри масиву всередині пари квадратних дужок `[]` після імені масиву. 

```cpp
int turnAngles[3];
```

Можна ініціалізувати значення елементів масиву під час створення масиву, використовуючи фігурні дужки.

```cpp
bool boolArray[2] = { false, true };
```

Значення можна присвоїти індивідуально за індексами. Індекс завжди починається з нуля.

```cpp
// Оголошення нового масиву завдовжки 3
double doubleArray[3];

// Присвоєння значень за індексом
double doubleArray[0] = 1.5;
double doubleArray[1] = 3.14;
double doubleArray[2] = 2.18;
```

Щоб зчитати значення з масиву, введіть індекс потрібного елемента у квадратних дужках.

```cpp
// Зчитує значення за індексом 2 в масиві integerArray

int value = integerArray[2];
```

## Приклад

У цьому прикладі ініціалізуються значення масиву, потім дістається елемент №3 (з індексом 2) зі списку, щоб обертати мотор.

```cpp
int degreesArray[3] = { 30, 60, 90 };
Motor.spinFor(forward, degreesArray[2], degrees);
```

<advanced>
</advanced>