category: sensing  
signature: VISION.objects[0].centerY  
device_class: vision  
description: Reports the Y coordinate of the center of a detected object from the Vision Sensor.

# Objects center Y

Повертає координату Y центру об'єкта, знайденого датчиком зору.

```cpp
Vision.objects[index].centerY
```

## Як це працює

Щоб використати `Vision.objects[index]`, виконайте наступні кроки:

1. Налаштуйте ваш датчик зору у вікні пристроїв.
2. Використайте `Vision.takeSnapshot()`, щоб захопити зображення з датчика зору і пошукати на ньому сигнатури або коди кольору.
3. Використайте `Vision.objects[index].exists`, щоб перевірити, чи датчик зору знайшов потрібну сигнатуру / коди кольору.

Щойно датчик зору побачить об'єкт, використайте інші блоки датчика зору, щоб дізнатися більше про об'єкт.

* Використайте **index** щоб вибрати об'єкт з усіх знайдених, про який ви хочете дізнатися більше. Більший об'єкт буде вище у списку,наприклад, `Vision.objects[0]` повертає найбільший об'єкт.
* Використайте `Vision.objectCount`, щоб визначити, скільки сигнатур / кодів кольору було знайдено.
* Додатково можна отримати таку інформацію про об'єкти: `angle`, `centerX`, `centerY`, `height`, `width` і `exists`.

---

`Vision.objects[index].centerY` повідомляє координату Y центру знайденого об'єкта. Повертає значення в діапазоні **0 - 211 px**.

```cpp
Brain.Screen.print(MyVision.objects[2].centerY);
```

<advanced>
</advanced>