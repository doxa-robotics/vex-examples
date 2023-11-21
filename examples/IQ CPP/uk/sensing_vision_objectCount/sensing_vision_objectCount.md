category: sensing  
signature: Vision.objectCount  
device_class: vision  
description: Reports how many objects the Vision Sensor detects. 

# Vision Object Count

Повідомляє, скільки об'єктів бачить датчик зору. 

```cpp
Vision.objectCount
```

## Як це працює

Переконайтеся, що ви вказали назву датчика зору в першій частині команди. 

Щоб команда `Vision.objectCount` могла знайти об'єкти, спочатку потрібно налаштувати сигнатуру кольору.

Спочатку треба викликати `Vision.takeSnapshot` для фотографування потрібної сигнатури, а потім `Vision.objectCount` зможе повідомити про кількість знайдених об'єктів.

`Vision.objectCount` повертає кількість об'єктів, знайдених на останній фотографії.

## Приклад

Приклад нижче друкує на екрані VEX IQ Brain кількість об'єктів обраної сигнатури, знайдених датчиком зору.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);

  // Зробити фотографію обраної сигнатури
  Vision.takeSnapshot(SIGNATURE);

  Brain.Screen.print("Number of Objects Detected: %d", Vision.objectCount);

  // Робити нову фотографію кожні 20 мілісекунд
  wait(20, msec);
}
```

<advanced>
</advanced>