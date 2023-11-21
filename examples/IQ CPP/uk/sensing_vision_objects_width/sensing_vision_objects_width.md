category: sensing  
signature: VISION.objects[0].width;  
device_class: vision  
description: Reports the width of a detected object from the Vision Sensor.

# Objects width

Повертає ширину об'єкта, знайденого датчиком зору.

```cpp
Vision.objects[index].width
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

`Vision.objects[index].width` повідомляє, наскільки широкий об'єкт у пікселях. Повертає значення в діапазоні **2 - 316 px**.

```cpp
Brain.Screen.print(MyVision.objects[1].width);
```

<advanced>
</advanced>