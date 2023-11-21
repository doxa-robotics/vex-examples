category: events  
signature: EVENT.broadcast();  
description: Broadcast event message to run listener functions.

# Broadcast

Надсилає повідомлення для активації будь-яких функцій, які викликані подією **Event**.

```cpp
myEvent.broadcast();
```

## Як це працює

Код програми продовжить виконуватися після команди `myEvent.broadcast`, тому вона працюватиме водначас із функціями прослуховувачами подій event listener.

Перед використанням цієї команди визначена подія має бути створена і прописана хоча б в одному зворотному виклику callback.

```cpp
void runOnBroadcast1() {
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Broadcast1 Running");
}

void runOnBroadcast2() {
  Brain.Screen.setCursor(2, 1);
  Brain.Screen.print("Broadcast2 Running");
}

int main() {
  // Створіть подію в головній функції main
  event myEvent = event();

  // Пропишіть функцію зворотного виклику в подію
  myEvent(runOnBroadcast1);
  myEvent(runOnBroadcast2);

  // Активуйте подію
  myEvent.broadcast();
}
```

<advanced>
</advanced>