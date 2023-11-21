category: events  
signature: events_brain_timer
description: Runs the specified function when the IQ Brain's timer is greater than the given value.

# Timer Event

Запускає функцію зворотного виклику через певний проміжок часу.

```cpp
Brain.Timer.event(callback, time);
```

## Як це працює

Таймер IQ Brain починає відлік після запуску кожної програми.

Функція `Brain.Timer.event` приймає 2 параметра.

Перший параметр - функція зворотного виклику (**callback function**). Цю функцію спочатку потрібно створити, щоб передати її у функцію `Brain.Timer.event`.

Другий параметр - час, через який запуститься функція зворотного виклику. Ця функція (**callback function**) запуститься, щойно час **Brain Timer** стане більшим за введене значення. Введений параметр `time` має бути в **мілісекундах**.

```cpp
// Функція зворотного виклику callback спрацює через 1000 мілісекунд
Brain.Timer.event(callback, 1000);
```

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**. 

У прикладі нижче надпис "Callback Function Called" буде надруковано на екрані VEX IQ Brain через 10 секунд.

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Timer.event(callbackFunction, 10000);
}
```

<advanced>
</advanced>