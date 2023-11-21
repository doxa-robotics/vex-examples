category: sensing  
signature: Vision.largestObject  
description: Reports the largest object that the vision sensor sees.

# Vision Largest Object

Повертає інформацію про найбільший знайдений датчиком зору об'єкт.

```cpp
Vision.largestObject
```

## Як це працює

Необхідно викликати команду `Vision.takeSnapshot` перед використанням команди `Vision.largestObject`.

Команда `Vision.largestObject` повертає об'єкт типу `vision::object`.

```cpp
// Зробити фото сигнатури кольору COLOR_SIG
Vision.takeSnapshot(COLOR_SIG);

Brain.Screen.print("X: %d", Vision.largestObject.centerX);
Brain.Screen.newLine();
Brain.Screen.print("Y: %d", Vision.largestObject.centerY);
Brain.Screen.newLine();
```

`Vision.largestObject` має тип `vision::object`, тому доступні такі властивості.

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