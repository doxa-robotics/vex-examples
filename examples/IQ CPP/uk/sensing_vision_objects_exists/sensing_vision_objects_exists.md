category: sensing  
signature: VISION.objects[0].exists;  
device_class: vision  
description: Reports if the Vision Sensor detects a configured object. 

# Objects exists

Повідомляє, якщо датчик зору знайшов заданий об'єкт. 

Об'єкт потрібно налаштувати, перш ніж команда `Vision.objects[index].exists` зможе його знайти.

```cpp
Vision.objects[index].exists
```

## Як це працює

Переконайтеся, що ви вказали назву датчика зору в першій частині команди. 

`Vision.objects[index].exists` повертає значення **true**, коли датчик зору знайшов заданий об'єкт.

`Vision.objects[index].exists` повертає значення **false**, коли датчик зору не знайшов заданий об'єкт.

Перед тим, як команда `Vision.objects[index].exists` зможе повернути значення **true** або **false**, необхідно використати `Vision.takeSnapshot()`.


```cpp
if(Vision.objects[0].exists){

}
```

<advanced>
</advanced>