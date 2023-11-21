category: drive  
signature: Drivetrain.turnFor(right, 90, degrees);  
device_class: drivetrain  
description: Turns the Drivetrain for a distance.  

# Turn For

Повертає трансмісію на певний кут та напрямок

```cpp
Drivetrain.turnFor(direction, angle, degrees);
```

## Як це працює

Задайте напрямок - `direction` - і кут повороту, ввівши напрямок - **left** або **right**, і кількість градусів.

```cpp
Drivetrain.turnFor(right, 270, degrees);
```

Команда `Drivetrain.turnFor` за замовчуванням блокує інші команди, поки трансмісія повертає.

## Необов'язкові параметри

Ви можете встановити значення останнього параметра `false`, щоб команда `Drivetrain.turnFor` не блокувала програму під час виконання руху.

```cpp
Drivetrain.turnFor(left, 90, degrees, false);
```

<advanced>
</advanced>
