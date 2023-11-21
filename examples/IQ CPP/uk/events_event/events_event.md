category: events  
signature: event myEvent = event(myEventCallback); 
description: Creates a new user event.

# Event

Створює нову подію, щоб активувати визначену функцію користувача.

```cpp
event myEvent = event(callbackFunction);
```

## Як це працює
Об'єкт **event** можна використати, щоб активувати функцію, визначену користувачем.Для роботи необхідно створити об'єкт **event**. Це можна зробити двома способами.

Функцію зворотного виклику (**callback function**) можна використати як аргумент для створеної функції.

```cpp
event myEvent = event(callbackFunction);
```
Функцію **callback function** не обов'язково передавати у новостворену функцію.

```cpp
event myEvent = event();
```
У подію можна додати декілька функцій **callback functions**. Всі вони спрацюють одночасно, коли виконається подія.

```cpp
event myEvent = event();
myEvent(callbackFunction1);
myEvent(callbackFunction1);
```
Лише **2 події функцій зворотного виклику** мають працювати водночас. Додаткові **події функцій зворотного виклику** можуть знизити продуктивність робота VEX IQ.

Функція зворотного виклику виконається, коли викликати або функцію `myEvent.broadcast`, або `myEvent.broadcastAndWait`.

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**.

```cpp
void callbackFunction() {
  Brain.Screen.print("Function Called.");
}

int main() {
  // Створення нової події з назвою myEvent у головній функції main і передавання callbackFunction
  event myEvent = event(callbackFunction);

  // Надсилання myEvent, активуючи виведення напису "Function Called." на екрані Brain
  myEvent.broadcast();
}
```

<advanced>
</advanced>