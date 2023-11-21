category: events  
signature: events_event_broadcast_and_wait   
description: Broadcast event message to run listener functions and wait for all listeners to finish before continuing.

# Broadcast and Wait

Надсилає повідомлення для активації будь-яких функцій, які викликані подією **Event**, а продовження програми зупиняється.

```cpp
myEvent.broadcastAndWait();
```

## Як це працює

Команда `myEvent.broadcastAndWait` чекає, поки всі прослуховувачі не виконаються, а потім продовжує роботу програми. Це зупиняє виконання коду поточної функції, поки всі надіслані прослуховувачі повністю не виконаються.

Перед використанням цієї команди визначена подія має бути створена і прописана хоча б в одному зворотному виклику callback.

## Функція зворотного виклику

Функція зворотного виклику - це функція, яка передається в іншу функцію як аргумент. Код всередині функції зворотного виклику (**callback function**) запрацює, коли виконається подія **event**.

```cpp
void callbackFunction() {
  Brain.Screen.print("Function Called.");

  wait(5, seconds);
}

int main() {
  // Пропишіть нову подію в головній функції main і передайте їй функцію callbackFunction
  event myEvent = event(callbackFunction);

  // Активуйте подію, програма чекає, поки подія не виконається
  myEvent.broadcastAndWait();

  // Ця частина не почнеться, поки callbackFunction не виконається
  Brain.Screen.newLine();
  Brain.Screen.print("Done!");
}
```

<advanced>
</advanced>