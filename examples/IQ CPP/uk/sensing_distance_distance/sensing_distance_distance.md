category: sensing  
signature: Distance.distance(units)  
device-class: sonar
description: Reports the distance of the nearest object from the VEX IQ Distance Sensor.

# Distance From

Передає відстань до найближчого об'єкта від датчика відстані VEX IQ.

```cpp
Distance.distance(units)
```

## Як це працює

`Distance.distance` передає значення в діапазоні **від 24 до 1000 мм** або **від 1 до 40 дюймів**.

Перша частина команди - назва пристрою.

```cpp
Distance6.distance(mm)
Distance8.distance(inches)
```

Встановіть, у яких одиницях повертатиме значення команда `Distance.distance`: **inches** або **mm** (міліметри). 

```cpp
Distance6.distance(mm)
Distance8.distance(inches)
```

<advanced>
</advanced>