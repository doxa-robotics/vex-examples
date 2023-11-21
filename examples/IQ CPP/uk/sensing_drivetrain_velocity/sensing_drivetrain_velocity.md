category: sensing  
signature: Drivetrain.velocity(units)  
device_class: drivetrain
description: Reports the current velocity of the Drivetrain.

# Drivetrain Velocity

Передає поточну швидкість трансмісії.

```cpp
Drivetrain.velocity(units)
```

## Як це працює
`Drivetrain.velocity` передає десяткове значення (*double*), яке показує поточну швидкість трансмісії.

`Drivetrain.velocity` передає значення в діапазоні **від -100% до 100%**, якщо одиниці вимірювання `units` - **percent**.

`Drivetrain.velocity` також передає значення в **rpm** (revolutions per minute - обертів за хвилину) якщо ввести ці одиниці в параметр `units`.

Якщо отримано негативне значення, це значить, що трансмісія рухається у зворотному напрямку.

## Приклад

Приклад нижче друкує швидкість трансмісії (у відсотках) на екрані VEX IQ Brain.

```cpp
Brain.Screen.print("%f", Drivetrain.velocity(percent));
```

<advanced>
</advanced>