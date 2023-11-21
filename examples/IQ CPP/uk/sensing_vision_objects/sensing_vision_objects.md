category: sensing  
signature: Vision.objects  
device_class: vision  
description: Reports the objects the Vision Sensor detects. 

# Vision Objects

Повертає масив з усіх об'єктів, які побачив датчик зору.

```cpp
Vision.objects
```

## Як це працює

Необхідно викликати команду `Vision.takeSnapshot` перед використанням масиву `Vision.objects`.

`Vision.objects` - це масив, який містить усі об'єкти, які знайшов датчик зору на останній фотографії.

```cpp
Vision.takeSnapshot(COLOR_SIG);
vision::object firstObject = Vision.objects[0];
```
Його можна використовувати як будь-який інший масив. Ви можете отримати доступ до об'єктів у ньому за індексом кожного елемента.

```cpp
vision::object visionObject = Vision.objects[0];
```

Ви також можете використати структури керування, наприклад **цикл for**. Команду `Vision.objectCount` можна використати як умову циклу.

Частина нижче друкує на VEX IQ Brain значення центрів `centerX` і `centerY` кожного знайденого об'єкта.

```cpp
Vision.takeSnapshot(COLOR_SIG);

for(int i = 0; i < Vision.objectCount; i++) {
  Brain.Screen.print("X: %d", Vision.objects[i].centerX);
  Brain.Screen.newLine();
  Brain.Screen.print("Y: %d", Vision.objects[i].centerY);
  Brain.Screen.newLine();
}
```

`Vision.objects` має тип `vision::object`, тому доступні такі властивості.

- `id` - Унікальний ID, присвоєний кожному об'єкту датчиком зору, тип `int`
- `originX` - Позиція верхньої лівої частини об'єкта по вісі X, тип `int`
- `originY` - Позиція верхньої лівої частини об'єкта по вісі Y, тип `int`
- `centerX` - Позиція центра об'єкта по вісі X, тип `int`
- `centerY` - Позиція центра об'єкта по вісі Y, тип `int`
- `width` - Ширина об'єкта, тип `int`
- `height` - Висота об'єкта, тип `int`
- `angle` - Кут об'єкта, тип `double`
- `exists` - Датчик зору бачить об'єкт або ні, тип `bool`


<advanced>
</advanced>