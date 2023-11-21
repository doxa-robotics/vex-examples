category: drive  
signature: Drivetrain.driveFor(forward, 1, inches);  
device_class: drivetrain  
description: Moves the Drivetrain for a given distance.  

# Drive For

Рухає трансмісію на задану відстань

```cpp
Drivetrain.driveFor(direction, distance, units);
```

## Як це працює

Виберіть напрямок - `direction` - руху трансмісії: **forward** або **reverse**. 

Встановіть відстань, яку проїде трансмісія, ввівши числове значення `distance`. 

Потім, визначте одиниці вимірювання `units`: **inches** або **mm**.

```cpp
Drivetrain.driveFor(reverse, 5, inches);
```

Команда `Drivetrain.driveFor` за замовчуванням блокує інші команди, поки трансмісія рухається.

## Необов'язкові параметри

Ви можете встановити значення останнього параметра `false`, щоб команда `Drivetrain.driveFor` не блокувала програму під час виконання руху.

```cpp
Drivetrain.driveFor(forward, 200, mm, false);
```

<advanced>
</advanced>
