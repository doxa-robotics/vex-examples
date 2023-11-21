category: functions  
signature: function_thread
description: Allows you to execute multiple threads at the same time.

# Thread

Дає змогу виконувати кілька потоків (threads) одночасно.

```cpp
thread myThread = thread(myThreadCallback);
```

## Як це працює

Треба визначити функцію, яку буде передано зворотнім викликом в потік.

```cpp
void myThreadCallback() {
  Brain.Screen.print("In a different thread!");
}
```
Щойно ви напишете функцію, можете використати її, щоб створити новий потік. Ця функія передається як функція зворотного виклику **callback function**.

```cpp
thread myThread = thread(myThreadCallback);
```
Потік **thread** почне виконуватись одразу після створення. Він працює паралельно з головним потоком.

Лише два потоки (**2 threads**) мають працювати водночас. Додаткові потоки можуть зменшити продуктивність робота VEX IQ.

## Приклад

Цей приклад надрукує одночасно два лічильника на екрані VEX IQ Brain. Один буде друкуватися потоком `myThread`. Інший тоді ж друкуватиметься основним потоком.

```cpp
void myThreadCallback() {
  int count = 0;
  while(true) {
    Brain.Screen.setCursor(1, 1);
    Brain.Screen.print("thread1: %d", count);
    count++;
    // Очікування для виконання основного потоку
    wait(25, msec);
  }
}

int main() {
  // Створений потік одразу почне виконання
  thread myThread = thread(myThreadCallback);
  
  int count = 0;
  while(true) {
    Brain.Screen.setCursor(2, 1);
    Brain.Screen.print("main: %d", count);
    count++;
    // Очікування для виконання myThread
    wait(25, msec);
  }
}
```

<advanced>
</advanced>
