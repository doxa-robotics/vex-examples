category: sensing  
signature: Gyro.setRotation(rotation, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current rotation to the value provided. 

# Gyro Set Rotation

Встановлює кут повороту гіродатчика VEX IQ в задане значення.

```cpp
Gyro.setRotation(rotation, degrees);
```

## Як це працює

Команду `Gyro.setRotation` використовують, щоб перезаписати поточну позицію кута повороту гіродатчика на введене позитивне (проти годинникової стрілки) або негативне (за годинниковою стрілкою) значення.

`Gyro.setRotation` приймає позицію в межах будь-якого негативного або позитивного десяткового чи цілого числа в параметр `rotation`.

## Приклад

Приклад нижче встановлює кут повороту гіродатчика в -45 градусів.

```cpp
Gyro.setRotation(-45, degrees);
```

<advanced>
</advanced>