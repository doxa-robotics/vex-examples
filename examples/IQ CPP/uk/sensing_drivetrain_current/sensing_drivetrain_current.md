category: sensing  
signature: Drivetrain.current(units)  
device_class: drivetrain  
description: Reports the amount of current (power) that the Drivetrain is currently using.

# Drivetrain Current

Передає кількість струму, яку зараз використовує трансмісія.

```cpp
Drivetrain.current(units)
```

## Як це працює
`Drivetrain.current` передає десяткове значення (*double*) кількості струму, яку зараз використовує трансмісія.

`Drivetrain.current` повертає значення відповідно до встановлених одиниць вимірювання `units`.

Можливі варіанти одиниць вимірювання `units` - **amp** (ампери) або **percent**.

## Приклад

Приклад нижче надрукує значення струму (в амперах) трансмісії робота VEX IQ на екрані Brain.

```cpp
Brain.Screen.print("%f", Drivetrain.current(amp));
```

<advanced>
</advanced>