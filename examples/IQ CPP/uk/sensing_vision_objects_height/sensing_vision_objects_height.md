category: sensing  
signature: VISION.objects[0].height;  
device_class: vision  
description: Reports the height of a detected object from the Vision Sensor.

# Objects height

Повертає висоту об'єкта, знайденого датчиком зору.

```cpp
Vision.objects[index].height
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

`Vision.objects[index].height` повідомляє, наскільки високий об'єкт у пікселях. Повертає значення в діапазоні **2 - 212 px**.

```cpp
Brain.Screen.print(MyVision.objects[3].height);
```

<advanced>
</advanced>