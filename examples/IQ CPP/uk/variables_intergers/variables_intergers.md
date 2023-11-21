category: variables 
signature: variables_intergers
description: Sets a variable to a `int` type.

# Integer Variable

Встановлює числову змінну з оголошенням ім'ям і значення.

`int myNumber = 10;`

## Як це працює

Створіть унікальне і характерне ім'я.

`int driveTime = 60;`

Присвойте значення змінній. Змінна може зберігати значення датчиків або результати обчислень, якщо вони мають відповідний **тип**.

```cpp
int lowBatteryLifeWarning = Brain.Battery.capacity(percent);
```


## Приклад

У цьому прикладі змінній "myVariable" присвоюється відстань (у міліметрах), отримана датчиком відстані VEX IQ, ця змінна "myVariable" використовується для встановлення швидкості трансмісії.

```cpp
int myVariable = Distance7.distance(mm);

Drivetrain.setDriveVelocity(myVariable, percent);
```

<advanced>
</advanced>